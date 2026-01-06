# Продвинутые примеры использования DialogData в T-Flex CAD API

## Расширенные сценарии работы с данными диалога

### 1. Создание параметризованных данных диалога

```csharp
// Параметризованные данные диалога с возможностью настройки
public static class AdvancedDialogData
{
    // Параметры для данных диалога
    public static class DialogDataSettings
    {
        public static int MinSteps = 1;
        public static int MaxSteps = 1000;
        public static int MinHoles = 0;
        public static int MaxHoles = 1000;
        public static bool EnableValidation = true;
        public static bool EnableLogging = true;
        public static int MaxHistorySize = 100;
        public static bool EnableAutoSave = true;
        public static TimeSpan AutoSaveInterval = TimeSpan.FromMinutes(5);
    }
    
    // Расширенные данные диалога с проверкой значений
    public class AdvancedDialogData : DialogData
    {
        public int MinSteps { get; set; } = DialogDataSettings.MinSteps;
        public int MaxSteps { get; set; } = DialogDataSettings.MaxSteps;
        public int MinHoles { get; set; } = DialogDataSettings.MinHoles;
        public int MaxHoles { get; set; } = DialogDataSettings.MaxHoles;
        public bool EnableValidation { get; set; } = DialogDataSettings.EnableValidation;
        public bool EnableLogging { get; set; } = DialogDataSettings.EnableLogging;
        public List<DialogDataHistory> History { get; set; } = new List<DialogDataHistory>();
        public int MaxHistorySize { get; set; } = DialogDataSettings.MaxHistorySize;
        public bool EnableAutoSave { get; set; } = DialogDataSettings.EnableAutoSave;
        public TimeSpan AutoSaveInterval { get; set; } = DialogDataSettings.AutoSaveInterval;
        public DateTime LastAutoSaveTime { get; set; } = DateTime.MinValue;
        
        public AdvancedDialogData()
        {
            MinSteps = DialogDataSettings.MinSteps;
            MaxSteps = DialogDataSettings.MaxSteps;
            MinHoles = DialogDataSettings.MinHoles;
            MaxHoles = DialogDataSettings.MaxHoles;
            MaxHistorySize = DialogDataSettings.MaxHistorySize;
            EnableAutoSave = DialogDataSettings.EnableAutoSave;
            AutoSaveInterval = DialogDataSettings.AutoSaveInterval;
        }
        
        public override List<ShaftStep> Steps
        {
            get => base.Steps;
            set
            {
                if (EnableValidation)
                {
                    ValidateSteps(value);
                }
                AddToHistory();
                base.Steps = value;
                
                // Автосохранение при изменении данных
                if (EnableAutoSave && ShouldAutoSave())
                {
                    AutoSave();
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get => base.Holes;
            set
            {
                if (EnableValidation)
                {
                    ValidateHoles(value);
                }
                AddToHistory();
                base.Holes = value;
                
                // Автосохранение при изменении данных
                if (EnableAutoSave && ShouldAutoSave())
                {
                    AutoSave();
                }
            }
        }
        
        public override ShaftStep SelectedStep
        {
            get => base.SelectedStep;
            set
            {
                AddToHistory();
                base.SelectedStep = value;
            }
        }
        
        public override ShaftHole SelectedHole
        {
            get => base.SelectedHole;
            set
            {
                AddToHistory();
                base.SelectedHole = value;
            }
        }
        
        private void ValidateSteps(List<ShaftStep> steps)
        {
            if (steps.Count < MinSteps)
            {
                throw new ArgumentOutOfRangeException(nameof(steps), 
                    $"Количество ступеней {steps.Count} меньше минимального допустимого значения {MinSteps}");
            }
            
            if (steps.Count > MaxSteps)
            {
                throw new ArgumentOutOfRangeException(nameof(steps), 
                    $"Количество ступеней {steps.Count} больше максимального допустимого значения {MaxSteps}");
            }
        }
        
        private void ValidateHoles(List<ShaftHole> holes)
        {
            if (holes.Count < MinHoles)
            {
                throw new ArgumentOutOfRangeException(nameof(holes), 
                    $"Количество отверстий {holes.Count} меньше минимального допустимого значения {MinHoles}");
            }
            
            if (holes.Count > MaxHoles)
            {
                throw new ArgumentOutOfRangeException(nameof(holes), 
                    $"Количество отверстий {holes.Count} больше максимального допустимого значения {MaxHoles}");
            }
        }
        
        public void LogOperation(string operation)
        {
            if (EnableLogging)
            {
                Console.WriteLine($"[DialogData] {operation}");
            }
        }
        
        public bool IsValidDialogData()
        {
            try
            {
                ValidateSteps(Steps);
                ValidateHoles(Holes);
                return true;
            }
            catch
            {
                return false;
            }
        }
        
        public DialogDataValidationResult ValidateDialogData()
        {
            var result = new DialogDataValidationResult();
            
            try
            {
                ValidateSteps(Steps);
                result.IsStepsValid = true;
            }
            catch (Exception ex)
            {
                result.IsStepsValid = false;
                result.StepsError = ex.Message;
            }
            
            try
            {
                ValidateHoles(Holes);
                result.IsHolesValid = true;
            }
            catch (Exception ex)
            {
                result.IsHolesValid = false;
                result.HolesError = ex.Message;
            }
            
            result.IsValid = result.IsStepsValid && result.IsHolesValid;
            return result;
        }
        
        private void AddToHistory()
        {
            var historyEntry = new DialogDataHistory
            {
                Timestamp = DateTime.Now,
                Steps = new List<ShaftStep>(base.Steps),
                Holes = new List<ShaftHole>(base.Holes),
                SelectedStep = base.SelectedStep,
                SelectedHole = base.SelectedHole,
                IsModified = true
            };
            
            History.Add(historyEntry);
            
            // Ограничение размера истории
            if (History.Count > MaxHistorySize)
            {
                History.RemoveAt(0);
            }
        }
        
        public List<DialogDataHistory> GetHistory()
        {
            return new List<DialogDataHistory>(History);
        }
        
        public void ClearHistory()
        {
            History.Clear();
        }
        
        public void RestoreFromHistory(DialogDataHistory historyEntry)
        {
            if (historyEntry != null)
            {
                base.Steps = new List<ShaftStep>(historyEntry.Steps);
                base.Holes = new List<ShaftHole>(historyEntry.Holes);
                base.SelectedStep = historyEntry.SelectedStep;
                base.SelectedHole = historyEntry.SelectedHole;
            }
        }
        
        private bool ShouldAutoSave()
        {
            return DateTime.Now - LastAutoSaveTime > AutoSaveInterval;
        }
        
        public void AutoSave()
        {
            // Реализация автосохранения данных диалога
            LastAutoSaveTime = DateTime.Now;
            LogOperation("Автосохранение данных диалога выполнено");
        }
        
        public void ForceSave()
        {
            // Принудительное сохранение данных диалога
            LastAutoSaveTime = DateTime.Now;
            LogOperation("Принудительное сохранение данных диалога выполнено");
        }
        
        public void LoadFromTemplate(string templateName)
        {
            // Загрузка данных диалога из шаблона
            LogOperation($"Загрузка данных диалога из шаблона: {templateName}");
        }
        
        public void SaveAsTemplate(string templateName)
        {
            // Сохранение данных диалога как шаблона
            LogOperation($"Сохранение данных диалога как шаблона: {templateName}");
        }
    }
    
    // Результат валидации данных диалога
    public class DialogDataValidationResult
    {
        public bool IsValid { get; set; } = true;
        public bool IsStepsValid { get; set; } = true;
        public bool IsHolesValid { get; set; } = true;
        public string StepsError { get; set; }
        public string HolesError { get; set; }
    }
    
    // История изменений данных диалога
    public class DialogDataHistory
    {
        public DateTime Timestamp { get; set; }
        public List<ShaftStep> Steps { get; set; }
        public List<ShaftHole> Holes { get; set; }
        public ShaftStep SelectedStep { get; set; }
        public ShaftHole SelectedHole { get; set; }
        public bool IsModified { get; set; } = true;
    }
    
    // Расширенные данные диалога с ограничениями
    public class ConstrainedDialogData : AdvancedDialogData
    {
        public int MinSteps { get; set; } = DialogDataSettings.MinSteps;
        public int MaxSteps { get; set; } = DialogDataSettings.MaxSteps;
        public int MinHoles { get; set; } = DialogDataSettings.MinHoles;
        public int MaxHoles { get; set; } = DialogDataSettings.MaxHoles;
        public bool EnableValidation { get; set; } = true;
        
        public ConstrainedDialogData()
        {
            MinSteps = DialogDataSettings.MinSteps;
            MaxSteps = DialogDataSettings.MaxSteps;
            MinHoles = DialogDataSettings.MinHoles;
            MaxHoles = DialogDataSettings.MaxHoles;
        }
        
        public override List<ShaftStep> Steps
        {
            get => base.Steps;
            set
            {
                if (EnableValidation)
                {
                    ValidateSteps(value);
                }
                base.Steps = value;
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get => base.Holes;
            set
            {
                if (EnableValidation)
                {
                    ValidateHoles(value);
                }
                base.Holes = value;
            }
        }
        
        private void ValidateSteps(List<ShaftStep> steps)
        {
            if (steps.Count < MinSteps)
            {
                throw new ArgumentOutOfRangeException(nameof(steps), 
                    $"Количество ступеней {steps.Count} меньше минимального допустимого значения {MinSteps}");
            }
            
            if (steps.Count > MaxSteps)
            {
                throw new ArgumentOutOfRangeException(nameof(steps), 
                    $"Количество ступеней {steps.Count} больше максимального допустимого значения {MaxSteps}");
            }
        }
        
        private void ValidateHoles(List<ShaftHole> holes)
        {
            if (holes.Count < MinHoles)
            {
                throw new ArgumentOutOfRangeException(nameof(holes), 
                    $"Количество отверстий {holes.Count} меньше минимального допустимого значения {MinHoles}");
            }
            
            if (holes.Count > MaxHoles)
            {
                throw new ArgumentOutOfRangeException(nameof(holes), 
                    $"Количество отверстий {holes.Count} больше максимального допустимого значения {MaxHoles}");
            }
        }
        
        public bool IsWithinConstraints()
        {
            try
            {
                ValidateSteps(Steps);
                ValidateHoles(Holes);
                return true;
            }
            catch
            {
                return false;
            }
        }
        
        public void EnforceConstraints()
        {
            // Принудительное соблюдение ограничений
            if (Steps.Count < MinSteps)
            {
                while (Steps.Count < MinSteps)
                {
                    Steps.Add(new ShaftStep());
                }
            }
            
            if (Steps.Count > MaxSteps)
            {
                Steps.RemoveRange(MaxSteps, Steps.Count - MaxSteps);
            }
            
            if (Holes.Count < MinHoles)
            {
                while (Holes.Count < MinHoles)
                {
                    Holes.Add(new ShaftHole());
                }
            }
            
            if (Holes.Count > MaxHoles)
            {
                Holes.RemoveRange(MaxHoles, Holes.Count - MaxHoles);
            }
        }
    }
}
```

### 2. Создание адаптивных данных диалога

```csharp
// Адаптивные данные диалога, которые автоматически настраиваются под параметры
public static class AdaptiveDialogData
{
    // Правила адаптации для данных диалога
    public static class AdaptationRules
    {
        public static DialogDataAdaptationType StepsRule = DialogDataAdaptationType.OptimizeForPerformance;
        public static DialogDataAdaptationType HolesRule = DialogDataAdaptationType.OptimizeForMemory;
        public static int MaxStepsForOptimization = 50;
        public static int MaxHolesForOptimization = 100;
        public static bool EnableLazyLoading = true;
        public static int LazyLoadThreshold = 10;
    }
    
    // Адаптивные данные диалога с автоматической адаптацией
    public class AdaptiveDialogData : DialogData
    {
        public DialogDataAdaptationType StepsAdaptationType { get; set; } = AdaptationRules.StepsRule;
        public DialogDataAdaptationType HolesAdaptationType { get; set; } = AdaptationRules.HolesRule;
        public int MaxStepsForOptimization { get; set; } = AdaptationRules.MaxStepsForOptimization;
        public int MaxHolesForOptimization { get; set; } = AdaptationRules.MaxHolesForOptimization;
        public bool EnableAdaptation { get; set; } = true;
        public bool EnableOptimization { get; set; } = true;
        public bool EnableLazyLoading { get; set; } = AdaptationRules.EnableLazyLoading;
        public int LazyLoadThreshold { get; set; } = AdaptationRules.LazyLoadThreshold;
        public Dictionary<int, ShaftStep> LazyLoadedSteps { get; set; } = new Dictionary<int, ShaftStep>();
        public Dictionary<int, ShaftHole> LazyLoadedHoles { get; set; } = new Dictionary<int, ShaftHole>();
        
        public AdaptiveDialogData()
        {
            StepsAdaptationType = AdaptationRules.StepsRule;
            HolesAdaptationType = AdaptationRules.HolesRule;
            MaxStepsForOptimization = AdaptationRules.MaxStepsForOptimization;
            MaxHolesForOptimization = AdaptationRules.MaxHolesForOptimization;
            EnableLazyLoading = AdaptationRules.EnableLazyLoading;
            LazyLoadThreshold = AdaptationRules.LazyLoadThreshold;
        }
        
        public override List<ShaftStep> Steps
        {
            get
            {
                if (EnableLazyLoading && base.Steps.Count > LazyLoadThreshold)
                {
                    return GetLazyLoadedSteps();
                }
                return base.Steps;
            }
            set
            {
                if (EnableAdaptation)
                {
                    base.Steps = AdaptSteps(value);
                }
                else
                {
                    base.Steps = value;
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get
            {
                if (EnableLazyLoading && base.Holes.Count > LazyLoadThreshold)
                {
                    return GetLazyLoadedHoles();
                }
                return base.Holes;
            }
            set
            {
                if (EnableAdaptation)
                {
                    base.Holes = AdaptHoles(value);
                }
                else
                {
                    base.Holes = value;
                }
            }
        }
        
        private List<ShaftStep> AdaptSteps(List<ShaftStep> steps)
        {
            switch (StepsAdaptationType)
            {
                case DialogDataAdaptationType.OptimizeForPerformance:
                    return OptimizeStepsForPerformance(steps);
                    
                case DialogDataAdaptationType.OptimizeForMemory:
                    return OptimizeStepsForMemory(steps);
                    
                case DialogDataAdaptationType.ApplyTarget:
                    return steps; // В реальной реализации здесь будет целевое значение
                    
                default:
                    return steps;
            }
        }
        
        private List<ShaftHole> AdaptHoles(List<ShaftHole> holes)
        {
            switch (HolesAdaptationType)
            {
                case DialogDataAdaptationType.OptimizeForPerformance:
                    return OptimizeHolesForPerformance(holes);
                    
                case DialogDataAdaptationType.OptimizeForMemory:
                    return OptimizeHolesForMemory(holes);
                    
                case DialogDataAdaptationType.ApplyTarget:
                    return holes; // В реальной реализации здесь будет целевое значение
                    
                default:
                    return holes;
            }
        }
        
        // Оптимизация ступеней для производительности
        private List<ShaftStep> OptimizeStepsForPerformance(List<ShaftStep> steps)
        {
            if (steps.Count > MaxStepsForOptimization)
            {
                // Оптимизация больших наборов данных
                return steps.Take(MaxStepsForOptimization).ToList();
            }
            return steps;
        }
        
        // Оптимизация ступеней для памяти
        private List<ShaftStep> OptimizeStepsForMemory(List<ShaftStep> steps)
        {
            if (steps.Count > MaxStepsForOptimization)
            {
                // Оптимизация больших наборов данных
                return steps.Take(MaxStepsForOptimization).ToList();
            }
            return steps;
        }
        
        // Оптимизация отверстий для производительности
        private List<ShaftHole> OptimizeHolesForPerformance(List<ShaftHole> holes)
        {
            if (holes.Count > MaxHolesForOptimization)
            {
                // Оптимизация больших наборов данных
                return holes.Take(MaxHolesForOptimization).ToList();
            }
            return holes;
        }
        
        // Оптимизация отверстий для памяти
        private List<ShaftHole> OptimizeHolesForMemory(List<ShaftHole> holes)
        {
            if (holes.Count > MaxHolesForOptimization)
            {
                // Оптимизация больших наборов данных
                return holes.Take(MaxHolesForOptimization).ToList();
            }
            return holes;
        }
        
        public bool IsOptimized()
        {
            return Steps.Count <= MaxStepsForOptimization && Holes.Count <= MaxHolesForOptimization;
        }
        
        public void OptimizeData()
        {
            Steps = AdaptSteps(Steps);
            Holes = AdaptHoles(Holes);
        }
        
        private List<ShaftStep> GetLazyLoadedSteps()
        {
            // Реализация ленивой загрузки ступеней
            List<ShaftStep> result = new List<ShaftStep>();
            
            for (int i = 0; i < base.Steps.Count; i++)
            {
                if (LazyLoadedSteps.ContainsKey(i))
                {
                    result.Add(LazyLoadedSteps[i]);
                }
                else
                {
                    // Загрузка данных по требованию
                    ShaftStep step = base.Steps[i];
                    LazyLoadedSteps[i] = step;
                    result.Add(step);
                }
            }
            
            return result;
        }
        
        private List<ShaftHole> GetLazyLoadedHoles()
        {
            // Реализация ленивой загрузки отверстий
            List<ShaftHole> result = new List<ShaftHole>();
            
            for (int i = 0; i < base.Holes.Count; i++)
            {
                if (LazyLoadedHoles.ContainsKey(i))
                {
                    result.Add(LazyLoadedHoles[i]);
                }
                else
                {
                    // Загрузка данных по требованию
                    ShaftHole hole = base.Holes[i];
                    LazyLoadedHoles[i] = hole;
                    result.Add(hole);
                }
            }
            
            return result;
        }
        
        public void ClearLazyLoadedData()
        {
            LazyLoadedSteps.Clear();
            LazyLoadedHoles.Clear();
        }
        
        public void PreloadData()
        {
            // Предварительная загрузка данных
            for (int i = 0; i < base.Steps.Count; i++)
            {
                if (!LazyLoadedSteps.ContainsKey(i))
                {
                    LazyLoadedSteps[i] = base.Steps[i];
                }
            }
            
            for (int i = 0; i < base.Holes.Count; i++)
            {
                if (!LazyLoadedHoles.ContainsKey(i))
                {
                    LazyLoadedHoles[i] = base.Holes[i];
                }
            }
        }
    }
    
    // Адаптивные данные диалога с контекстом
    public class ContextualDialogData : AdaptiveDialogData
    {
        public DialogDataContext Context { get; set; }
        public Dictionary<DialogDataContext, DialogData> ContextData { get; set; } = new Dictionary<DialogDataContext, DialogData>();
        
        public ContextualDialogData()
        {
            Context = DialogDataContext.Default;
        }
        
        public override List<ShaftStep> Steps
        {
            get
            {
                if (ContextData.ContainsKey(Context) && ContextData[Context] != null)
                {
                    return ContextData[Context].Steps;
                }
                return base.Steps;
            }
            set
            {
                if (ContextData.ContainsKey(Context))
                {
                    ContextData[Context].Steps = value;
                }
                else
                {
                    ContextData[Context] = new DialogData { Steps = value };
                }
                
                if (Context == DialogDataContext.Default)
                {
                    base.Steps = value;
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get
            {
                if (ContextData.ContainsKey(Context) && ContextData[Context] != null)
                {
                    return ContextData[Context].Holes;
                }
                return base.Holes;
            }
            set
            {
                if (ContextData.ContainsKey(Context))
                {
                    ContextData[Context].Holes = value;
                }
                else
                {
                    ContextData[Context] = new DialogData { Holes = value };
                }
                
                if (Context == DialogDataContext.Default)
                {
                    base.Holes = value;
                }
            }
        }
        
        public void SetDataForContext(DialogDataContext context, DialogData data)
        {
            ContextData[context] = data;
        }
        
        public DialogData GetDataForContext(DialogDataContext context)
        {
            return ContextData.ContainsKey(context) ? ContextData[context] : null;
        }
        
        public void SwitchContext(DialogDataContext newContext)
        {
            Context = newContext;
        }
        
        public List<DialogDataContext> GetAvailableContexts()
        {
            return ContextData.Keys.ToList();
        }
    }
    
    // Адаптивные данные диалога с историей изменений
    public class HistoricalDialogData : ContextualDialogData
    {
        public List<DialogDataHistory> History { get; set; } = new List<DialogDataHistory>();
        public int MaxHistorySize { get; set; } = 100;
        public bool EnableHistory { get; set; } = true;
        
        public HistoricalDialogData()
        {
            MaxHistorySize = 100;
        }
        
        public override List<ShaftStep> Steps
        {
            get => base.Steps;
            set
            {
                if (EnableHistory)
                {
                    AddToHistory();
                }
                base.Steps = value;
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get => base.Holes;
            set
            {
                if (EnableHistory)
                {
                    AddToHistory();
                }
                base.Holes = value;
            }
        }
        
        private void AddToHistory()
        {
            var historyEntry = new DialogDataHistory
            {
                Timestamp = DateTime.Now,
                Steps = new List<ShaftStep>(base.Steps),
                Holes = new List<ShaftHole>(base.Holes),
                SelectedStep = base.SelectedStep,
                SelectedHole = base.SelectedHole,
                Context = Context
            };
            
            History.Add(historyEntry);
            
            // Ограничение размера истории
            if (History.Count > MaxHistorySize)
            {
                History.RemoveAt(0);
            }
        }
        
        public List<DialogDataHistory> GetHistoryForContext(DialogDataContext context)
        {
            return History.Where(h => h.Context == context).ToList();
        }
        
        public List<DialogDataHistory> GetRecentHistory(int count)
        {
            return History.TakeLast(count).ToList();
        }
        
        public void ClearHistory()
        {
            History.Clear();
        }
        
        public void RestoreFromHistory(DialogDataHistory historyEntry)
        {
            if (historyEntry != null)
            {
                base.Steps = new List<ShaftStep>(historyEntry.Steps);
                base.Holes = new List<ShaftHole>(historyEntry.Holes);
                base.SelectedStep = historyEntry.SelectedStep;
                base.SelectedHole = historyEntry.SelectedHole;
                Context = historyEntry.Context;
            }
        }
    }
}

// Контекст данных диалога
public enum DialogDataContext
{
    Default,
    Design,
    Analysis,
    Manufacturing,
    Inspection
}

// Правила адаптации данных диалога
public enum DialogDataAdaptationType
{
    None,
    OptimizeForPerformance,
    OptimizeForMemory,
    ApplyTarget
}
```

### 3. Создание данных диалога с условной логикой

```csharp
// Данные диалога с условной логикой на основе контекста
public static class ConditionalDialogData
{
    // Условия для данных диалога
    public static List<DialogDataCondition> Conditions { get; set; } = new List<DialogDataCondition>();
    
    // Стратегии для данных диалога
    public static Dictionary<DialogDataOperationType, DialogDataOperationStrategy> Strategies { get; set; } 
        = new Dictionary<DialogDataOperationType, DialogDataOperationStrategy>();
    
    // Добавление условия
    public static void AddCondition(DialogDataCondition condition)
    {
        Conditions.Add(condition);
    }
    
    // Добавление стратегии
    public static void AddStrategy(DialogDataOperationType type, DialogDataOperationStrategy strategy)
    {
        Strategies[type] = strategy;
    }
    
    // Условные данные диалога с автоматическим выбором стратегии
    public class ConditionalDialogData : DialogData
    {
        public DialogDataContext Context { get; set; }
        public bool EnableConditionalLogic { get; set; } = true;
        
        public ConditionalDialogData()
        {
            Context = DialogDataContext.Default;
        }
        
        public override List<ShaftStep> Steps
        {
            get
            {
                if (EnableConditionalLogic)
                {
                    return GetConditionalSteps();
                }
                return base.Steps;
            }
            set
            {
                if (EnableConditionalLogic)
                {
                    SetConditionalSteps(value);
                }
                else
                {
                    base.Steps = value;
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get
            {
                if (EnableConditionalLogic)
                {
                    return GetConditionalHoles();
                }
                return base.Holes;
            }
            set
            {
                if (EnableConditionalLogic)
                {
                    SetConditionalHoles(value);
                }
                else
                {
                    base.Holes = value;
                }
            }
        }
        
        private List<ShaftStep> GetConditionalSteps()
        {
            // Определение типа операции на основе условий
            DialogDataOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                return Strategies[operationType].GetSteps(this);
            }
            
            // Если стратегия не найдена, возвращаем базовые ступени
            return base.Steps;
        }
        
        private void SetConditionalSteps(List<ShaftStep> steps)
        {
            // Определение типа операции на основе условий
            DialogDataOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                Strategies[operationType].SetSteps(this, steps);
            }
            else
            {
                // Если стратегия не найдена, используем стандартное присвоение
                base.Steps = steps;
            }
        }
        
        private List<ShaftHole> GetConditionalHoles()
        {
            // Определение типа операции на основе условий
            DialogDataOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                return Strategies[operationType].GetHoles(this);
            }
            
            // Если стратегия не найдена, возвращаем базовые отверстия
            return base.Holes;
        }
        
        private void SetConditionalHoles(List<ShaftHole> holes)
        {
            // Определение типа операции на основе условий
            DialogDataOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                Strategies[operationType].SetHoles(this, holes);
            }
            else
            {
                // Если стратегия не найдена, используем стандартное присвоение
                base.Holes = holes;
            }
        }
        
        private DialogDataOperationType DetermineOperationType()
        {
            // Проверка условий
            foreach (var condition in Conditions)
            {
                if (CheckCondition(condition))
                {
                    return condition.OperationType;
                }
            }
            
            // Если ни одно условие не выполнено, возвращаем тип по умолчанию
            return DialogDataOperationType.Standard;
        }
        
        private bool CheckCondition(DialogDataCondition condition)
        {
            switch (condition.Parameter)
            {
                case ConditionalDialogDataParameter.Context:
                    return (int)Context == condition.Value;
                case ConditionalDialogDataParameter.StepsCount:
                    return base.Steps.Count >= condition.Value;
                case ConditionalDialogDataParameter.HolesCount:
                    return base.Holes.Count >= condition.Value;
                default:
                    return false;
            }
        }
    }
    
    // Условные данные диалога с множественными значениями
    public class MultiValueDialogData : ConditionalDialogData
    {
        public Dictionary<DialogDataContext, DialogData> Values { get; set; } = new Dictionary<DialogDataContext, DialogData>();
        
        public MultiValueDialogData()
        {
            Values[DialogDataContext.Default] = new DialogData();
        }
        
        public override List<ShaftStep> Steps
        {
            get
            {
                if (Values.ContainsKey(Context))
                {
                    return Values[Context].Steps;
                }
                return base.Steps;
            }
            set
            {
                if (!Values.ContainsKey(Context))
                {
                    Values[Context] = new DialogData();
                }
                Values[Context].Steps = value;
                
                if (Context == DialogDataContext.Default)
                {
                    base.Steps = value;
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get
            {
                if (Values.ContainsKey(Context))
                {
                    return Values[Context].Holes;
                }
                return base.Holes;
            }
            set
            {
                if (!Values.ContainsKey(Context))
                {
                    Values[Context] = new DialogData();
                }
                Values[Context].Holes = value;
                
                if (Context == DialogDataContext.Default)
                {
                    base.Holes = value;
                }
            }
        }
        
        public void SetValueForContext(DialogDataContext context, DialogData value)
        {
            Values[context] = value;
        }
        
        public DialogData GetValueForContext(DialogDataContext context)
        {
            return Values.ContainsKey(context) ? Values[context] : null;
        }
        
        public void RemoveValueForContext(DialogDataContext context)
        {
            if (Values.ContainsKey(context))
            {
                Values.Remove(context);
            }
        }
    }
    
    // Условные данные диалога с вычисляемыми значениями
    public class ComputedDialogData : ConditionalDialogData
    {
        public Func<DialogDataContext, List<ShaftStep>> StepsComputationFunction { get; set; }
        public Func<DialogDataContext, List<ShaftHole>> HolesComputationFunction { get; set; }
        public bool EnableComputation { get; set; } = true;
        public List<ShaftStep> CachedSteps { get; set; }
        public List<ShaftHole> CachedHoles { get; set; }
        public DateTime LastComputationTime { get; set; }
        public TimeSpan CacheTimeout { get; set; } = TimeSpan.FromMinutes(5);
        
        public ComputedDialogData()
        {
            CacheTimeout = TimeSpan.FromMinutes(5);
        }
        
        public override List<ShaftStep> Steps
        {
            get
            {
                if (EnableComputation && StepsComputationFunction != null)
                {
                    // Проверка необходимости пересчета
                    if (IsCacheExpired())
                    {
                        CachedSteps = StepsComputationFunction(Context);
                        LastComputationTime = DateTime.Now;
                    }
                    return CachedSteps;
                }
                return base.Steps;
            }
            set
            {
                if (EnableConditionalLogic)
                {
                    SetConditionalSteps(value);
                }
                else
                {
                    base.Steps = value;
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get
            {
                if (EnableComputation && HolesComputationFunction != null)
                {
                    // Проверка необходимости пересчета
                    if (IsCacheExpired())
                    {
                        CachedHoles = HolesComputationFunction(Context);
                        LastComputationTime = DateTime.Now;
                    }
                    return CachedHoles;
                }
                return base.Holes;
            }
            set
            {
                if (EnableConditionalLogic)
                {
                    SetConditionalHoles(value);
                }
                else
                {
                    base.Holes = value;
                }
            }
        }
        
        private bool IsCacheExpired()
        {
            return DateTime.Now - LastComputationTime > CacheTimeout;
        }
        
        public void InvalidateCache()
        {
            LastComputationTime = DateTime.MinValue;
            CachedSteps = null;
            CachedHoles = null;
        }
        
        public void SetStepsComputationFunction(Func<DialogDataContext, List<ShaftStep>> function)
        {
            StepsComputationFunction = function;
            InvalidateCache();
        }
        
        public void SetHolesComputationFunction(Func<DialogDataContext, List<ShaftHole>> function)
        {
            HolesComputationFunction = function;
            InvalidateCache();
        }
    }
    
    // Стандартная стратегия
    public static class StandardStrategy : DialogDataOperationStrategy
    {
        public override List<ShaftStep> GetSteps(ConditionalDialogData data)
        {
            return data.BaseSteps;
        }
        
        public override void SetSteps(ConditionalDialogData data, List<ShaftStep> steps)
        {
            data.BaseSteps = steps;
        }
        
        public override List<ShaftHole> GetHoles(ConditionalDialogData data)
        {
            return data.BaseHoles;
        }
        
        public override void SetHoles(ConditionalDialogData data, List<ShaftHole> holes)
        {
            data.BaseHoles = holes;
        }
    }
    
    // Высокоточная стратегия
    public static class HighPrecisionStrategy : DialogDataOperationStrategy
    {
        public override List<ShaftStep> GetSteps(ConditionalDialogData data)
        {
            // Получение ступеней с высокой точностью
            return data.BaseSteps.Select(s => new ShaftStep 
            { 
                Diameter = Math.Round(s.Diameter, 3),
                Length = Math.Round(s.Length, 3),
                PrimitiveType = s.PrimitiveType
            }).ToList();
        }
        
        public override void SetSteps(ConditionalDialogData data, List<ShaftStep> steps)
        {
            // Установка ступеней с высокой точностью
            data.BaseSteps = steps.Select(s => new ShaftStep 
            { 
                Diameter = Math.Round(s.Diameter, 3),
                Length = Math.Round(s.Length, 3),
                PrimitiveType = s.PrimitiveType
            }).ToList();
        }
        
        public override List<ShaftHole> GetHoles(ConditionalDialogData data)
        {
            // Получение отверстий с высокой точностью
            return data.BaseHoles.Select(h => new ShaftHole 
            { 
                Diameter = Math.Round(h.Diameter, 3),
                Depth = Math.Round(h.Depth, 3),
                Position = h.Position
            }).ToList();
        }
        
        public override void SetHoles(ConditionalDialogData data, List<ShaftHole> holes)
        {
            // Установка отверстий с высокой точностью
            data.BaseHoles = holes.Select(h => new ShaftHole 
            { 
                Diameter = Math.Round(h.Diameter, 3),
                Depth = Math.Round(h.Depth, 3),
                Position = h.Position
            }).ToList();
        }
    }
    
    // Оптимизированная стратегия
    public static class OptimizedStrategy : DialogDataOperationStrategy
    {
        public override List<ShaftStep> GetSteps(ConditionalDialogData data)
        {
            // Получение оптимизированных ступеней
            return data.BaseSteps;
        }
        
        public override void SetSteps(ConditionalDialogData data, List<ShaftStep> steps)
        {
            // Установка оптимизированных ступеней
            data.BaseSteps = steps;
        }
        
        public override List<ShaftHole> GetHoles(ConditionalDialogData data)
        {
            // Получение оптимизированных отверстий
            return data.BaseHoles;
        }
        
        public override void SetHoles(ConditionalDialogData data, List<ShaftHole> holes)
        {
            // Установка оптимизированных отверстий
            data.BaseHoles = holes;
        }
    }
    
    // Расширение базовых данных диалога для условных данных
    public class ConditionalDialogData : DialogData
    {
        public List<ShaftStep> BaseSteps { get; set; } = new List<ShaftStep>();
        public List<ShaftHole> BaseHoles { get; set; } = new List<ShaftHole>();
        
        public override List<ShaftStep> Steps
        {
            get => BaseSteps;
            set => BaseSteps = value;
        }
        
        public override List<ShaftHole> Holes
        {
            get => BaseHoles;
            set => BaseHoles = value;
        }
    }
}

// Условие для данных диалога
public class DialogDataCondition
{
    public ConditionalDialogDataParameter Parameter { get; set; }
    public ComparisonOperator Operator { get; set; }
    public double Value { get; set; }
    public DialogDataOperationType OperationType { get; set; }
}

public enum ConditionalDialogDataParameter
{
    Context,
    StepsCount,
    HolesCount,
    Complexity
}

public enum DialogDataOperationType
{
    Standard,
    HighPrecision,
    Optimized,
    Debug
}

// Абстрактная стратегия для данных диалога
public abstract class DialogDataOperationStrategy
{
    public abstract List<ShaftStep> GetSteps(ConditionalDialogData data);
    public abstract void SetSteps(ConditionalDialogData data, List<ShaftStep> steps);
    public abstract List<ShaftHole> GetHoles(ConditionalDialogData data);
    public abstract void SetHoles(ConditionalDialogData data, List<ShaftHole> holes);
}
```

### 4. Создание данных диалога с множественными конфигурациями

```csharp
// Данные диалога с множественными конфигурациями
public static class MultiConfigurationDialogData
{
    // Конфигурации для данных диалога
    public static List<DialogDataConfiguration> Configurations { get; set; } = new List<DialogDataConfiguration>();
    public static int CurrentConfigurationIndex { get; set; } = 0;
    
    // Добавление конфигурации
    public static void AddConfiguration(DialogDataConfiguration config)
    {
        Configurations.Add(config);
    }
    
    // Получение текущей конфигурации
    public static DialogDataConfiguration GetCurrentConfiguration()
    {
        if (Configurations.Count == 0)
            return null;
            
        if (CurrentConfigurationIndex >= 0 && CurrentConfigurationIndex < Configurations.Count)
        {
            return Configurations[CurrentConfigurationIndex];
        }
        
        return Configurations[0];
    }
    
    // Переключение на следующую конфигурацию
    public static DialogDataConfiguration SwitchToNextConfiguration()
    {
        if (Configurations.Count == 0)
            return null;
            
        CurrentConfigurationIndex = (CurrentConfigurationIndex + 1) % Configurations.Count;
        return GetCurrentConfiguration();
    }
    
    // Переключение на предыдущую конфигурацию
    public static DialogDataConfiguration SwitchToPreviousConfiguration()
    {
        if (Configurations.Count == 0)
            return null;
            
        CurrentConfigurationIndex = (CurrentConfigurationIndex - 1 + Configurations.Count) % Configurations.Count;
        return GetCurrentConfiguration();
    }
    
    // Получение конфигурации по индексу
    public static DialogDataConfiguration GetConfigurationByIndex(int index)
    {
        if (index >= 0 && index < Configurations.Count)
        {
            CurrentConfigurationIndex = index;
            return Configurations[index];
        }
        
        return null;
    }
    
    // Данные диалога с множественными конфигурациями
    public class ConfigurableDialogData : DialogData
    {
        public Dictionary<DialogDataConfiguration, DialogData> ConfigurationValues { get; set; } 
            = new Dictionary<DialogDataConfiguration, DialogData>();
        public bool EnableConfigurationSwitching { get; set; } = true;
        
        public ConfigurableDialogData()
        {
            ConfigurationValues[new DialogDataConfiguration { Name = "Default", IsDefault = true }] = new DialogData();
        }
        
        public override List<ShaftStep> Steps
        {
            get
            {
                var currentConfig = MultiConfigurationDialogData.GetCurrentConfiguration();
                if (currentConfig != null && ConfigurationValues.ContainsKey(currentConfig))
                {
                    return ConfigurationValues[currentConfig].Steps;
                }
                return base.Steps;
            }
            set
            {
                var currentConfig = MultiConfigurationDialogData.GetCurrentConfiguration();
                if (currentConfig != null)
                {
                    if (!ConfigurationValues.ContainsKey(currentConfig))
                    {
                        ConfigurationValues[currentConfig] = new DialogData();
                    }
                    ConfigurationValues[currentConfig].Steps = value;
                }
                
                if (currentConfig?.IsDefault == true)
                {
                    base.Steps = value;
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get
            {
                var currentConfig = MultiConfigurationDialogData.GetCurrentConfiguration();
                if (currentConfig != null && ConfigurationValues.ContainsKey(currentConfig))
                {
                    return ConfigurationValues[currentConfig].Holes;
                }
                return base.Holes;
            }
            set
            {
                var currentConfig = MultiConfigurationDialogData.GetCurrentConfiguration();
                if (currentConfig != null)
                {
                    if (!ConfigurationValues.ContainsKey(currentConfig))
                    {
                        ConfigurationValues[currentConfig] = new DialogData();
                    }
                    ConfigurationValues[currentConfig].Holes = value;
                }
                
                if (currentConfig?.IsDefault == true)
                {
                    base.Holes = value;
                }
            }
        }
        
        public void SetValueForConfiguration(DialogDataConfiguration config, DialogData value)
        {
            ConfigurationValues[config] = value;
        }
        
        public DialogData GetValueForConfiguration(DialogDataConfiguration config)
        {
            return ConfigurationValues.ContainsKey(config) ? ConfigurationValues[config] : null;
        }
        
        public void RemoveConfigurationValue(DialogDataConfiguration config)
        {
            if (ConfigurationValues.ContainsKey(config))
            {
                ConfigurationValues.Remove(config);
            }
        }
        
        public List<DialogDataConfiguration> GetConfigurationsWithValues()
        {
            return ConfigurationValues.Keys.ToList();
        }
    }
    
    // Данные диалога с режимами работы
    public class ModeDialogData : ConfigurableDialogData
    {
        public DialogDataMode CurrentMode { get; set; } = DialogDataMode.Standard;
        public Dictionary<DialogDataMode, DialogData> ModeValues { get; set; } = new Dictionary<DialogDataMode, DialogData>();
        
        public ModeDialogData()
        {
            ModeValues[DialogDataMode.Standard] = new DialogData();
        }
        
        public override List<ShaftStep> Steps
        {
            get
            {
                if (ModeValues.ContainsKey(CurrentMode))
                {
                    return ModeValues[CurrentMode].Steps;
                }
                return base.Steps;
            }
            set
            {
                if (!ModeValues.ContainsKey(CurrentMode))
                {
                    ModeValues[CurrentMode] = new DialogData();
                }
                ModeValues[CurrentMode].Steps = value;
                
                if (CurrentMode == DialogDataMode.Standard)
                {
                    base.Steps = value;
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get
            {
                if (ModeValues.ContainsKey(CurrentMode))
                {
                    return ModeValues[CurrentMode].Holes;
                }
                return base.Holes;
            }
            set
            {
                if (!ModeValues.ContainsKey(CurrentMode))
                {
                    ModeValues[CurrentMode] = new DialogData();
                }
                ModeValues[CurrentMode].Holes = value;
                
                if (CurrentMode == DialogDataMode.Standard)
                {
                    base.Holes = value;
                }
            }
        }
        
        public void SetValueForMode(DialogDataMode mode, DialogData value)
        {
            ModeValues[mode] = value;
        }
        
        public DialogData GetValueForMode(DialogDataMode mode)
        {
            return ModeValues.ContainsKey(mode) ? ModeValues[mode] : null;
        }
        
        public void SwitchMode(DialogDataMode newMode)
        {
            CurrentMode = newMode;
        }
        
        public List<DialogDataMode> GetAvailableModes()
        {
            return ModeValues.Keys.ToList();
        }
    }
    
    // Данные диалога с профилями
    public class ProfileDialogData : ModeDialogData
    {
        public string CurrentProfile { get; set; } = "Default";
        public Dictionary<string, DialogData> ProfileValues { get; set; } = new Dictionary<string, DialogData>();
        
        public ProfileDialogData()
        {
            ProfileValues["Default"] = new DialogData();
        }
        
        public override List<ShaftStep> Steps
        {
            get
            {
                if (ProfileValues.ContainsKey(CurrentProfile))
                {
                    return ProfileValues[CurrentProfile].Steps;
                }
                return base.Steps;
            }
            set
            {
                if (!ProfileValues.ContainsKey(CurrentProfile))
                {
                    ProfileValues[CurrentProfile] = new DialogData();
                }
                ProfileValues[CurrentProfile].Steps = value;
                
                if (CurrentProfile == "Default")
                {
                    base.Steps = value;
                }
            }
        }
        
        public override List<ShaftHole> Holes
        {
            get
            {
                if (ProfileValues.ContainsKey(CurrentProfile))
                {
                    return ProfileValues[CurrentProfile].Holes;
                }
                return base.Holes;
            }
            set
            {
                if (!ProfileValues.ContainsKey(CurrentProfile))
                {
                    ProfileValues[CurrentProfile] = new DialogData();
                }
                ProfileValues[CurrentProfile].Holes = value;
                
                if (CurrentProfile == "Default")
                {
                    base.Holes = value;
                }
            }
        }
        
        public void SetValueForProfile(string profile, DialogData value)
        {
            ProfileValues[profile] = value;
        }
        
        public DialogData GetValueForProfile(string profile)
        {
            return ProfileValues.ContainsKey(profile) ? ProfileValues[profile] : null;
        }
        
        public void SwitchProfile(string newProfile)
        {
            CurrentProfile = newProfile;
        }
        
        public List<string> GetAvailableProfiles()
        {
            return ProfileValues.Keys.ToList();
        }
        
        public void AddProfile(string profile, DialogData value)
        {
            ProfileValues[profile] = value;
        }
        
        public void RemoveProfile(string profile)
        {
            if (ProfileValues.ContainsKey(profile))
            {
                ProfileValues.Remove(profile);
            }
        }
    }
}

// Конфигурация данных диалога
public class DialogDataConfiguration
{
    public string Name { get; set; }
    public string Description { get; set; }
    public bool IsDefault { get; set; } = false;
    public DialogDataSettings Settings { get; set; }
    public DialogDataOptimizationLevel OptimizationLevel { get; set; }
    
    public DialogDataConfiguration()
    {
        Settings = new DialogDataSettings();
    }
}

// Настройки данных диалога
public class DialogDataSettings
{
    public int MinSteps { get; set; } = 1;
    public int MaxSteps { get; set; } = 1000;
    public int MinHoles { get; set; } = 0;
    public int MaxHoles { get; set; } = 1000;
    public bool EnableLogging { get; set; } = true;
    public bool EnableValidation { get; set; } = true;
}

public enum DialogDataOptimizationLevel
{
    None,
    Basic,
    Advanced,
    Maximum
}

// Режимы данных диалога
public enum DialogDataMode
{
    Standard,
    HighPrecision,
    Optimized,
    Debug
}

// Пример использования множественных конфигураций данных диалога
public static void UseMultiConfigurationDialogData()
{
    // Конфигурация 1: Стандартная
    DialogDataConfiguration config1 = new DialogDataConfiguration();
    config1.Name = "Стандартная конфигурация";
    config1.Description = "Стандартные настройки данных диалога";
    config1.IsDefault = true;
    config1.Settings.EnableLogging = true;
    config1.Settings.EnableValidation = true;
    config1.OptimizationLevel = DialogDataOptimizationLevel.Basic;
    MultiConfigurationDialogData.AddConfiguration(config1);
    
    // Конфигурация 2: Оптимизированная
    DialogDataConfiguration config2 = new DialogDataConfiguration();
    config2.Name = "Оптимизированная конфигурация";
    config2.Description = "Оптимизированные настройки данных диалога";
    config2.Settings.EnableLogging = false;
    config2.Settings.EnableValidation = true;
    config2.OptimizationLevel = DialogDataOptimizationLevel.Advanced;
    MultiConfigurationDialogData.AddConfiguration(config2);
    
    // Конфигурация 3: Отладочная
    DialogDataConfiguration config3 = new DialogDataConfiguration();
    config3.Name = "Отладочная конфигурация";
    config3.Description = "Настройки данных диалога для отладки";
    config3.Settings.EnableLogging = true;
    config3.Settings.EnableValidation = true;
    config3.OptimizationLevel = DialogDataOptimizationLevel.None;
    MultiConfigurationDialogData.AddConfiguration(config3);
    
    Console.WriteLine("Множественные конфигурации данных диалога настроены");
}
```

## Практические рекомендации

1. Используйте параметризованные данные диалога для создания гибких решений
2. При создании адаптивных данных диалога учитывайте контекст использования
3. Используйте условные данные диалога для автоматического выбора стратегии выполнения
4. При создании данных диалога с множественными конфигурациями реализуйте систему переключения
5. Реализуйте проверки ограничений при установке значений данных диалога
6. Используйте логирование для отслеживания изменений данных диалога
7. При работе с множественными конфигурациями реализуйте систему описаний
8. Учитывайте ограничения T-Flex CAD API при создании данных диалога
9. Реализуйте обработку ошибок для повышения надежности данных диалога
10. Используйте стратегии для реализации различных подходов к работе с данными диалога