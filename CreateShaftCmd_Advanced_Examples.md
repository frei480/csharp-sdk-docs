# Продвинутые примеры использования CreateShaftCmd в T-Flex CAD API

## Расширенные сценарии работы с командой создания вала

### 1. Создание параметризованной команды создания вала

```csharp
// Параметризованная команда создания вала с возможностью настройки
public static class AdvancedCreateShaftCmd
{
    // Параметры для команды создания вала
    public static class CreateShaftCmdSettings
    {
        public static int MinSteps = 1;
        public static int MaxSteps = 1000;
        public static int MinHoles = 0;
        public static int MaxHoles = 1000;
        public static int MinElements = 0;
        public static int MaxElements = 1000;
        public static double MinDiameter = 0.1;
        public static double MaxDiameter = 10000;
        public static double MinLength = 0.1;
        public static double MaxLength = 50000;
        public static bool EnableValidation = true;
        public static bool EnableLogging = true;
        public static int MaxHistorySize = 100;
        public static bool EnableAutoSave = true;
        public static TimeSpan AutoSaveInterval = TimeSpan.FromMinutes(5);
        public static bool EnableCaching = true;
        public static TimeSpan CacheTimeout = TimeSpan.FromMinutes(10);
        public static bool EnableProgressTracking = true;
        public static int ProgressUpdateInterval = 100; // миллисекунды
    }
    
    // Расширенная команда создания вала с проверкой значений
    public class AdvancedCreateShaftCmd : CreateShaftCmd
    {
        public int MinSteps { get; set; } = CreateShaftCmdSettings.MinSteps;
        public int MaxSteps { get; set; } = CreateShaftCmdSettings.MaxSteps;
        public int MinHoles { get; set; } = CreateShaftCmdSettings.MinHoles;
        public int MaxHoles { get; set; } = CreateShaftCmdSettings.MaxHoles;
        public int MinElements { get; set; } = CreateShaftCmdSettings.MinElements;
        public int MaxElements { get; set; } = CreateShaftCmdSettings.MaxElements;
        public double MinDiameter { get; set; } = CreateShaftCmdSettings.MinDiameter;
        public double MaxDiameter { get; set; } = CreateShaftCmdSettings.MaxDiameter;
        public double MinLength { get; set; } = CreateShaftCmdSettings.MinLength;
        public double MaxLength { get; set; } = CreateShaftCmdSettings.MaxLength;
        public bool EnableValidation { get; set; } = CreateShaftCmdSettings.EnableValidation;
        public bool EnableLogging { get; set; } = CreateShaftCmdSettings.EnableLogging;
        public List<CreateShaftCmdHistory> History { get; set; } = new List<CreateShaftCmdHistory>();
        public int MaxHistorySize { get; set; } = CreateShaftCmdSettings.MaxHistorySize;
        public bool EnableAutoSave { get; set; } = CreateShaftCmdSettings.EnableAutoSave;
        public TimeSpan AutoSaveInterval { get; set; } = CreateShaftCmdSettings.AutoSaveInterval;
        public DateTime LastAutoSaveTime { get; set; } = DateTime.MinValue;
        public bool EnableCaching { get; set; } = CreateShaftCmdSettings.EnableCaching;
        public TimeSpan CacheTimeout { get; set; } = CreateShaftCmdSettings.CacheTimeout;
        public DateTime LastCacheUpdateTime { get; set; } = DateTime.MinValue;
        public CreateShaftCmd CachedCmd { get; set; }
        public bool EnableProgressTracking { get; set; } = CreateShaftCmdSettings.EnableProgressTracking;
        public int ProgressUpdateInterval { get; set; } = CreateShaftCmdSettings.ProgressUpdateInterval;
        public event EventHandler<ProgressEventArgs> ProgressChanged;
        public event EventHandler<StatusEventArgs> StatusChanged;
        public CreateShaftCmdStatus CurrentStatus { get; private set; } = CreateShaftCmdStatus.Idle;
        
        public AdvancedCreateShaftCmd()
        {
            MinSteps = CreateShaftCmdSettings.MinSteps;
            MaxSteps = CreateShaftCmdSettings.MaxSteps;
            MinHoles = CreateShaftCmdSettings.MinHoles;
            MaxHoles = CreateShaftCmdSettings.MaxHoles;
            MinElements = CreateShaftCmdSettings.MinElements;
            MaxElements = CreateShaftCmdSettings.MaxElements;
            MinDiameter = CreateShaftCmdSettings.MinDiameter;
            MaxDiameter = CreateShaftCmdSettings.MaxDiameter;
            MinLength = CreateShaftCmdSettings.MinLength;
            MaxLength = CreateShaftCmdSettings.MaxLength;
            MaxHistorySize = CreateShaftCmdSettings.MaxHistorySize;
            EnableAutoSave = CreateShaftCmdSettings.EnableAutoSave;
            AutoSaveInterval = CreateShaftCmdSettings.AutoSaveInterval;
            EnableCaching = CreateShaftCmdSettings.EnableCaching;
            CacheTimeout = CreateShaftCmdSettings.CacheTimeout;
            EnableProgressTracking = CreateShaftCmdSettings.EnableProgressTracking;
            ProgressUpdateInterval = CreateShaftCmdSettings.ProgressUpdateInterval;
        }
        
        public override void Run()
        {
            try
            {
                SetStatus(CreateShaftCmdStatus.Running);
                LogOperation("Запуск команды создания вала");
                
                if (EnableValidation)
                {
                    ValidateShaftData();
                }
                
                AddToHistory();
                
                // Отслеживание прогресса
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(0, "Начало создания вала"));
                }
                
                // Вызов базовой реализации
                base.Run();
                
                // Автосохранение при успешном выполнении
                if (EnableAutoSave && ShouldAutoSave())
                {
                    AutoSave();
                }
                
                SetStatus(CreateShaftCmdStatus.Completed);
                LogOperation("Команда создания вала успешно выполнена");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(100, "Создание вала завершено"));
                }
            }
            catch (Exception ex)
            {
                SetStatus(CreateShaftCmdStatus.Error);
                LogOperation($"Ошибка при выполнении команды создания вала: {ex.Message}");
                throw;
            }
        }
        
        public override void CreateShaft()
        {
            try
            {
                SetStatus(CreateShaftCmdStatus.CreatingShaft);
                LogOperation("Создание вала");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(10, "Создание вала"));
                }
                
                // Вызов базовой реализации
                base.CreateShaft();
                
                SetStatus(CreateShaftCmdStatus.ShaftCreated);
                LogOperation("Вал успешно создан");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(30, "Вал создан"));
                }
            }
            catch (Exception ex)
            {
                SetStatus(CreateShaftCmdStatus.Error);
                LogOperation($"Ошибка при создании вала: {ex.Message}");
                throw;
            }
        }
        
        public override void CreatePrimitives()
        {
            try
            {
                SetStatus(CreateShaftCmdStatus.CreatingPrimitives);
                LogOperation("Создание примитивов");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(30, "Создание примитивов"));
                }
                
                // Вызов базовой реализации
                base.CreatePrimitives();
                
                SetStatus(CreateShaftCmdStatus.PrimitivesCreated);
                LogOperation("Примитивы успешно созданы");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(50, "Примитивы созданы"));
                }
            }
            catch (Exception ex)
            {
                SetStatus(CreateShaftCmdStatus.Error);
                LogOperation($"Ошибка при создании примитивов: {ex.Message}");
                throw;
            }
        }
        
        public override void CreateLCS()
        {
            try
            {
                SetStatus(CreateShaftCmdStatus.CreatingLCS);
                LogOperation("Создание локальных систем координат");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(50, "Создание LCS"));
                }
                
                // Вызов базовой реализации
                base.CreateLCS();
                
                SetStatus(CreateShaftCmdStatus.LCSCreated);
                LogOperation("Локальные системы координат успешно созданы");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(70, "LCS созданы"));
                }
            }
            catch (Exception ex)
            {
                SetStatus(CreateShaftCmdStatus.Error);
                LogOperation($"Ошибка при создании LCS: {ex.Message}");
                throw;
            }
        }
        
        public override void CreateVariablesInFragment()
        {
            try
            {
                SetStatus(CreateShaftCmdStatus.CreatingVariables);
                LogOperation("Создание переменных во фрагменте");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(70, "Создание переменных"));
                }
                
                // Вызов базовой реализации
                base.CreateVariablesInFragment();
                
                SetStatus(CreateShaftCmdStatus.VariablesCreated);
                LogOperation("Переменные успешно созданы");
                
                if (EnableProgressTracking)
                {
                    OnProgressChanged(new ProgressEventArgs(90, "Переменные созданы"));
                }
            }
            catch (Exception ex)
            {
                SetStatus(CreateShaftCmdStatus.Error);
                LogOperation($"Ошибка при создании переменных: {ex.Message}");
                throw;
            }
        }
        
        private void ValidateShaftData()
        {
            // Проверка данных вала
            if (ShaftData == null)
            {
                throw new InvalidOperationException("Данные вала не заданы");
            }
            
            if (ShaftData.Steps.Count < MinSteps)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Steps), 
                    $"Количество ступеней {ShaftData.Steps.Count} меньше минимального допустимого значения {MinSteps}");
            }
            
            if (ShaftData.Steps.Count > MaxSteps)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Steps), 
                    $"Количество ступеней {ShaftData.Steps.Count} больше максимального допустимого значения {MaxSteps}");
            }
            
            // Проверка диаметров и длин ступеней
            foreach (var step in ShaftData.Steps)
            {
                if (step.Diameter < MinDiameter)
                {
                    throw new ArgumentOutOfRangeException(nameof(step.Diameter), 
                        $"Диаметр ступени {step.Diameter} меньше минимального допустимого значения {MinDiameter}");
                }
                
                if (step.Diameter > MaxDiameter)
                {
                    throw new ArgumentOutOfRangeException(nameof(step.Diameter), 
                        $"Диаметр ступени {step.Diameter} больше максимального допустимого значения {MaxDiameter}");
                }
                
                if (step.Length < MinLength)
                {
                    throw new ArgumentOutOfRangeException(nameof(step.Length), 
                        $"Длина ступени {step.Length} меньше минимального допустимого значения {MinLength}");
                }
                
                if (step.Length > MaxLength)
                {
                    throw new ArgumentOutOfRangeException(nameof(step.Length), 
                        $"Длина ступени {step.Length} больше максимального допустимого значения {MaxLength}");
                }
            }
            
            // Проверка отверстий
            if (ShaftData.Holes.Count < MinHoles)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Holes), 
                    $"Количество отверстий {ShaftData.Holes.Count} меньше минимального допустимого значения {MinHoles}");
            }
            
            if (ShaftData.Holes.Count > MaxHoles)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Holes), 
                    $"Количество отверстий {ShaftData.Holes.Count} больше максимального допустимого значения {MaxHoles}");
            }
            
            // Проверка элементов
            if (ShaftData.Elements.Count < MinElements)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Elements), 
                    $"Количество элементов {ShaftData.Elements.Count} меньше минимального допустимого значения {MinElements}");
            }
            
            if (ShaftData.Elements.Count > MaxElements)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Elements), 
                    $"Количество элементов {ShaftData.Elements.Count} больше максимального допустимого значения {MaxElements}");
            }
        }
        
        public void LogOperation(string operation)
        {
            if (EnableLogging)
            {
                Console.WriteLine($"[CreateShaftCmd] {operation}");
            }
        }
        
        public bool IsValidShaftData()
        {
            try
            {
                ValidateShaftData();
                return true;
            }
            catch
            {
                return false;
            }
        }
        
        public CreateShaftCmdValidationResult ValidateCommand()
        {
            var result = new CreateShaftCmdValidationResult();
            
            try
            {
                ValidateShaftData();
                result.IsDataValid = true;
            }
            catch (Exception ex)
            {
                result.IsDataValid = false;
                result.DataError = ex.Message;
            }
            
            result.IsValid = result.IsDataValid;
            return result;
        }
        
        private void AddToHistory()
        {
            var historyEntry = new CreateShaftCmdHistory
            {
                Timestamp = DateTime.Now,
                ShaftData = ShaftData != null ? new ShaftData(ShaftData) : null,
                Status = CurrentStatus,
                IsModified = true
            };
            
            History.Add(historyEntry);
            
            // Ограничение размера истории
            if (History.Count > MaxHistorySize)
            {
                History.RemoveAt(0);
            }
        }
        
        public List<CreateShaftCmdHistory> GetHistory()
        {
            return new List<CreateShaftCmdHistory>(History);
        }
        
        public void ClearHistory()
        {
            History.Clear();
        }
        
        public void RestoreFromHistory(CreateShaftCmdHistory historyEntry)
        {
            if (historyEntry != null && historyEntry.ShaftData != null)
            {
                ShaftData = new ShaftData(historyEntry.ShaftData);
                InvalidateCache();
            }
        }
        
        private bool ShouldAutoSave()
        {
            return DateTime.Now - LastAutoSaveTime > AutoSaveInterval;
        }
        
        public void AutoSave()
        {
            // Реализация автосохранения команды создания вала
            LastAutoSaveTime = DateTime.Now;
            LogOperation("Автосохранение команды создания вала выполнено");
        }
        
        public void ForceSave()
        {
            // Принудительное сохранение команды создания вала
            LastAutoSaveTime = DateTime.Now;
            LogOperation("Принудительное сохранение команды создания вала выполнено");
        }
        
        public void LoadFromTemplate(string templateName)
        {
            // Загрузка команды создания вала из шаблона
            LogOperation($"Загрузка команды создания вала из шаблона: {templateName}");
        }
        
        public void SaveAsTemplate(string templateName)
        {
            // Сохранение команды создания вала как шаблона
            LogOperation($"Сохранение команды создания вала как шаблона: {templateName}");
        }
        
        private bool IsCacheExpired()
        {
            return DateTime.Now - LastCacheUpdateTime > CacheTimeout;
        }
        
        private void InvalidateCache()
        {
            CachedCmd = null;
            LastCacheUpdateTime = DateTime.MinValue;
        }
        
        public void UpdateCache()
        {
            if (EnableCaching)
            {
                CachedCmd = new CreateShaftCmd
                {
                    ShaftData = ShaftData != null ? new ShaftData(ShaftData) : null
                };
                LastCacheUpdateTime = DateTime.Now;
            }
        }
        
        public CreateShaftCmd GetCachedCmd()
        {
            if (EnableCaching && CachedCmd != null && !IsCacheExpired())
            {
                return CachedCmd;
            }
            return null;
        }
        
        protected virtual void OnProgressChanged(ProgressEventArgs e)
        {
            ProgressChanged?.Invoke(this, e);
        }
        
        protected virtual void OnStatusChanged(StatusEventArgs e)
        {
            StatusChanged?.Invoke(this, e);
        }
        
        private void SetStatus(CreateShaftCmdStatus status)
        {
            if (CurrentStatus != status)
            {
                var oldStatus = CurrentStatus;
                CurrentStatus = status;
                OnStatusChanged(new StatusEventArgs(oldStatus, CurrentStatus));
            }
        }
        
        public void Cancel()
        {
            SetStatus(CreateShaftCmdStatus.Cancelled);
            LogOperation("Команда создания вала отменена");
        }
        
        public void Reset()
        {
            SetStatus(CreateShaftCmdStatus.Idle);
            LogOperation("Команда создания вала сброшена");
        }
        
        public CreateShaftCmdStatus GetStatus()
        {
            return CurrentStatus;
        }
    }
    
    // Результат валидации команды создания вала
    public class CreateShaftCmdValidationResult
    {
        public bool IsValid { get; set; } = true;
        public bool IsDataValid { get; set; } = true;
        public string DataError { get; set; }
    }
    
    // История изменений команды создания вала
    public class CreateShaftCmdHistory
    {
        public DateTime Timestamp { get; set; }
        public ShaftData ShaftData { get; set; }
        public CreateShaftCmdStatus Status { get; set; }
        public bool IsModified { get; set; } = true;
    }
    
    // Расширенная команда создания вала с ограничениями
    public class ConstrainedCreateShaftCmd : AdvancedCreateShaftCmd
    {
        public int MinSteps { get; set; } = CreateShaftCmdSettings.MinSteps;
        public int MaxSteps { get; set; } = CreateShaftCmdSettings.MaxSteps;
        public int MinHoles { get; set; } = CreateShaftCmdSettings.MinHoles;
        public int MaxHoles { get; set; } = CreateShaftCmdSettings.MaxHoles;
        public int MinElements { get; set; } = CreateShaftCmdSettings.MinElements;
        public int MaxElements { get; set; } = CreateShaftCmdSettings.MaxElements;
        public double MinDiameter { get; set; } = CreateShaftCmdSettings.MinDiameter;
        public double MaxDiameter { get; set; } = CreateShaftCmdSettings.MaxDiameter;
        public double MinLength { get; set; } = CreateShaftCmdSettings.MinLength;
        public double MaxLength { get; set; } = CreateShaftCmdSettings.MaxLength;
        public bool EnableValidation { get; set; } = true;
        
        public ConstrainedCreateShaftCmd()
        {
            MinSteps = CreateShaftCmdSettings.MinSteps;
            MaxSteps = CreateShaftCmdSettings.MaxSteps;
            MinHoles = CreateShaftCmdSettings.MinHoles;
            MaxHoles = CreateShaftCmdSettings.MaxHoles;
            MinElements = CreateShaftCmdSettings.MinElements;
            MaxElements = CreateShaftCmdSettings.MaxElements;
            MinDiameter = CreateShaftCmdSettings.MinDiameter;
            MaxDiameter = CreateShaftCmdSettings.MaxDiameter;
            MinLength = CreateShaftCmdSettings.MinLength;
            MaxLength = CreateShaftCmdSettings.MaxLength;
        }
        
        private void ValidateShaftData()
        {
            // Проверка данных вала
            if (ShaftData == null)
            {
                throw new InvalidOperationException("Данные вала не заданы");
            }
            
            if (ShaftData.Steps.Count < MinSteps)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Steps), 
                    $"Количество ступеней {ShaftData.Steps.Count} меньше минимального допустимого значения {MinSteps}");
            }
            
            if (ShaftData.Steps.Count > MaxSteps)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Steps), 
                    $"Количество ступеней {ShaftData.Steps.Count} больше максимального допустимого значения {MaxSteps}");
            }
            
            // Проверка диаметров и длин ступеней
            foreach (var step in ShaftData.Steps)
            {
                if (step.Diameter < MinDiameter)
                {
                    throw new ArgumentOutOfRangeException(nameof(step.Diameter), 
                        $"Диаметр ступени {step.Diameter} меньше минимального допустимого значения {MinDiameter}");
                }
                
                if (step.Diameter > MaxDiameter)
                {
                    throw new ArgumentOutOfRangeException(nameof(step.Diameter), 
                        $"Диаметр ступени {step.Diameter} больше максимального допустимого значения {MaxDiameter}");
                }
                
                if (step.Length < MinLength)
                {
                    throw new ArgumentOutOfRangeException(nameof(step.Length), 
                        $"Длина ступени {step.Length} меньше минимального допустимого значения {MinLength}");
                }
                
                if (step.Length > MaxLength)
                {
                    throw new ArgumentOutOfRangeException(nameof(step.Length), 
                        $"Длина ступени {step.Length} больше максимального допустимого значения {MaxLength}");
                }
            }
            
            // Проверка отверстий
            if (ShaftData.Holes.Count < MinHoles)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Holes), 
                    $"Количество отверстий {ShaftData.Holes.Count} меньше минимального допустимого значения {MinHoles}");
            }
            
            if (ShaftData.Holes.Count > MaxHoles)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Holes), 
                    $"Количество отверстий {ShaftData.Holes.Count} больше максимального допустимого значения {MaxHoles}");
            }
            
            // Проверка элементов
            if (ShaftData.Elements.Count < MinElements)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Elements), 
                    $"Количество элементов {ShaftData.Elements.Count} меньше минимального допустимого значения {MinElements}");
            }
            
            if (ShaftData.Elements.Count > MaxElements)
            {
                throw new ArgumentOutOfRangeException(nameof(ShaftData.Elements), 
                    $"Количество элементов {ShaftData.Elements.Count} больше максимального допустимого значения {MaxElements}");
            }
        }
        
        public bool IsWithinConstraints()
        {
            try
            {
                ValidateShaftData();
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
            if (ShaftData != null)
            {
                if (ShaftData.Steps.Count < MinSteps)
                {
                    while (ShaftData.Steps.Count < MinSteps)
                    {
                        ShaftData.Steps.Add(new ShaftStep());
                    }
                }
                
                if (ShaftData.Steps.Count > MaxSteps)
                {
                    ShaftData.Steps.RemoveRange(MaxSteps, ShaftData.Steps.Count - MaxSteps);
                }
                
                if (ShaftData.Holes.Count < MinHoles)
                {
                    while (ShaftData.Holes.Count < MinHoles)
                    {
                        ShaftData.Holes.Add(new ShaftHole());
                    }
                }
                
                if (ShaftData.Holes.Count > MaxHoles)
                {
                    ShaftData.Holes.RemoveRange(MaxHoles, ShaftData.Holes.Count - MaxHoles);
                }
                
                if (ShaftData.Elements.Count < MinElements)
                {
                    while (ShaftData.Elements.Count < MinElements)
                    {
                        ShaftData.Elements.Add(new Element());
                    }
                }
                
                if (ShaftData.Elements.Count > MaxElements)
                {
                    ShaftData.Elements.RemoveRange(MaxElements, ShaftData.Elements.Count - MaxElements);
                }
            }
        }
    }
}
```

### 2. Создание адаптивной команды создания вала

```csharp
// Адаптивная команда создания вала, которая автоматически настраивается под параметры
public static class AdaptiveCreateShaftCmd
{
    // Правила адаптации для команды создания вала
    public static class AdaptationRules
    {
        public static CreateShaftCmdAdaptationType StepsRule = CreateShaftCmdAdaptationType.OptimizeForPerformance;
        public static CreateShaftCmdAdaptationType HolesRule = CreateShaftCmdAdaptationType.OptimizeForMemory;
        public static CreateShaftCmdAdaptationType ElementsRule = CreateShaftCmdAdaptationType.OptimizeForStorage;
        public static int MaxStepsForOptimization = 50;
        public static int MaxHolesForOptimization = 100;
        public static int MaxElementsForOptimization = 200;
        public static bool EnableLazyLoading = true;
        public static int LazyLoadThreshold = 10;
        public static bool EnableDataCompression = true;
        public static CompressionLevel CompressionLevel = CompressionLevel.Optimal;
        public static bool EnableParallelProcessing = true;
        public static int MaxDegreeOfParallelism = 4;
    }
    
    // Адаптивная команда создания вала с автоматической адаптацией
    public class AdaptiveCreateShaftCmd : CreateShaftCmd
    {
        public CreateShaftCmdAdaptationType StepsAdaptationType { get; set; } = AdaptationRules.StepsRule;
        public CreateShaftCmdAdaptationType HolesAdaptationType { get; set; } = AdaptationRules.HolesRule;
        public CreateShaftCmdAdaptationType ElementsAdaptationType { get; set; } = AdaptationRules.ElementsRule;
        public int MaxStepsForOptimization { get; set; } = AdaptationRules.MaxStepsForOptimization;
        public int MaxHolesForOptimization { get; set; } = AdaptationRules.MaxHolesForOptimization;
        public int MaxElementsForOptimization { get; set; } = AdaptationRules.MaxElementsForOptimization;
        public bool EnableAdaptation { get; set; } = true;
        public bool EnableOptimization { get; set; } = true;
        public bool EnableLazyLoading { get; set; } = AdaptationRules.EnableLazyLoading;
        public int LazyLoadThreshold { get; set; } = AdaptationRules.LazyLoadThreshold;
        public Dictionary<int, ShaftStep> LazyLoadedSteps { get; set; } = new Dictionary<int, ShaftStep>();
        public Dictionary<int, ShaftHole> LazyLoadedHoles { get; set; } = new Dictionary<int, ShaftHole>();
        public Dictionary<int, Element> LazyLoadedElements { get; set; } = new Dictionary<int, Element>();
        public bool EnableDataCompression { get; set; } = AdaptationRules.EnableDataCompression;
        public CompressionLevel CompressionLevel { get; set; } = AdaptationRules.CompressionLevel;
        public byte[] CompressedData { get; set; }
        public DateTime LastCompressionTime { get; set; } = DateTime.MinValue;
        public TimeSpan CompressionInterval { get; set; } = TimeSpan.FromMinutes(30);
        public bool EnableParallelProcessing { get; set; } = AdaptationRules.EnableParallelProcessing;
        public int MaxDegreeOfParallelism { get; set; } = AdaptationRules.MaxDegreeOfParallelism;
        public CreateShaftCmdPerformanceProfile PerformanceProfile { get; set; } = CreateShaftCmdPerformanceProfile.Balanced;
        public CreateShaftCmdResourceUsage ResourceUsage { get; set; } = CreateShaftCmdResourceUsage.Moderate;
        
        public AdaptiveCreateShaftCmd()
        {
            StepsAdaptationType = AdaptationRules.StepsRule;
            HolesAdaptationType = AdaptationRules.HolesRule;
            ElementsAdaptationType = AdaptationRules.ElementsRule;
            MaxStepsForOptimization = AdaptationRules.MaxStepsForOptimization;
            MaxHolesForOptimization = AdaptationRules.MaxHolesForOptimization;
            MaxElementsForOptimization = AdaptationRules.MaxElementsForOptimization;
            EnableLazyLoading = AdaptationRules.EnableLazyLoading;
            LazyLoadThreshold = AdaptationRules.LazyLoadThreshold;
            EnableDataCompression = AdaptationRules.EnableDataCompression;
            CompressionLevel = AdaptationRules.CompressionLevel;
            CompressionInterval = TimeSpan.FromMinutes(30);
            EnableParallelProcessing = AdaptationRules.EnableParallelProcessing;
            MaxDegreeOfParallelism = AdaptationRules.MaxDegreeOfParallelism;
        }
        
        public override void Run()
        {
            try
            {
                // Адаптация под текущие параметры
                if (EnableAdaptation)
                {
                    AdaptToCurrentParameters();
                }
                
                // Оптимизация данных
                if (EnableOptimization)
                {
                    OptimizeData();
                }
                
                // Вызов базовой реализации
                base.Run();
            }
            catch (Exception ex)
            {
                LogOperation($"Ошибка при выполнении адаптивной команды создания вала: {ex.Message}");
                throw;
            }
        }
        
        public override void CreateShaft()
        {
            try
            {
                // Параллельная обработка при включенной опции
                if (EnableParallelProcessing && ShaftData != null)
                {
                    CreateShaftParallel();
                }
                else
                {
                    // Вызов базовой реализации
                    base.CreateShaft();
                }
            }
            catch (Exception ex)
            {
                LogOperation($"Ошибка при создании вала: {ex.Message}");
                throw;
            }
        }
        
        private void CreateShaftParallel()
        {
            if (ShaftData == null) return;
            
            // Создание примитивов параллельно
            if (ShaftData.Steps != null && ShaftData.Steps.Count > 0)
            {
                var options = new ParallelOptions { MaxDegreeOfParallelism = MaxDegreeOfParallelism };
                Parallel.ForEach(ShaftData.Steps, options, step =>
                {
                    // Создание примитива для каждой ступени
                    CreatePrimitiveForStep(step);
                });
            }
            
            // Создание LCS
            CreateLCS();
            
            // Создание переменных
            CreateVariablesInFragment();
        }
        
        private void CreatePrimitiveForStep(ShaftStep step)
        {
            // Реализация создания примитива для ступени
            // В реальной реализации здесь будет создание ModelObject
        }
        
        public override void CreatePrimitives()
        {
            try
            {
                // Ленивая загрузка при включенной опции
                if (EnableLazyLoading && ShaftData != null && 
                    (ShaftData.Steps.Count > LazyLoadThreshold || 
                     ShaftData.Holes.Count > LazyLoadThreshold || 
                     ShaftData.Elements.Count > LazyLoadThreshold))
                {
                    CreatePrimitivesWithLazyLoading();
                }
                else
                {
                    // Вызов базовой реализации
                    base.CreatePrimitives();
                }
            }
            catch (Exception ex)
            {
                LogOperation($"Ошибка при создании примитивов: {ex.Message}");
                throw;
            }
        }
        
        private void CreatePrimitivesWithLazyLoading()
        {
            if (ShaftData == null) return;
            
            // Ленивая загрузка ступеней
            var steps = GetLazyLoadedSteps();
            
            // Ленивая загрузка отверстий
            var holes = GetLazyLoadedHoles();
            
            // Ленивая загрузка элементов
            var elements = GetLazyLoadedElements();
            
            // Создание примитивов для загруженных данных
            foreach (var step in steps)
            {
                CreatePrimitiveForStep(step);
            }
        }
        
        private List<ShaftStep> GetLazyLoadedSteps()
        {
            if (ShaftData == null) return new List<ShaftStep>();
            
            // Реализация ленивой загрузки ступеней
            List<ShaftStep> result = new List<ShaftStep>();
            
            for (int i = 0; i < ShaftData.Steps.Count; i++)
            {
                if (LazyLoadedSteps.ContainsKey(i))
                {
                    result.Add(LazyLoadedSteps[i]);
                }
                else
                {
                    // Загрузка данных по требованию
                    ShaftStep step = ShaftData.Steps[i];
                    LazyLoadedSteps[i] = step;
                    result.Add(step);
                }
            }
            
            return result;
        }
        
        private List<ShaftHole> GetLazyLoadedHoles()
        {
            if (ShaftData == null) return new List<ShaftHole>();
            
            // Реализация ленивой загрузки отверстий
            List<ShaftHole> result = new List<ShaftHole>();
            
            for (int i = 0; i < ShaftData.Holes.Count; i++)
            {
                if (LazyLoadedHoles.ContainsKey(i))
                {
                    result.Add(LazyLoadedHoles[i]);
                }
                else
                {
                    // Загрузка данных по требованию
                    ShaftHole hole = ShaftData.Holes[i];
                    LazyLoadedHoles[i] = hole;
                    result.Add(hole);
                }
            }
            
            return result;
        }
        
        private List<Element> GetLazyLoadedElements()
        {
            if (ShaftData == null) return new List<Element>();
            
            // Реализация ленивой загрузки элементов
            List<Element> result = new List<Element>();
            
            for (int i = 0; i < ShaftData.Elements.Count; i++)
            {
                if (LazyLoadedElements.ContainsKey(i))
                {
                    result.Add(LazyLoadedElements[i]);
                }
                else
                {
                    // Загрузка данных по требованию
                    Element element = ShaftData.Elements[i];
                    LazyLoadedElements[i] = element;
                    result.Add(element);
                }
            }
            
            return result;
        }
        
        private void AdaptToCurrentParameters()
        {
            if (ShaftData == null) return;
            
            // Адаптация под количество ступеней
            if (ShaftData.Steps.Count > MaxStepsForOptimization)
            {
                StepsAdaptationType = CreateShaftCmdAdaptationType.OptimizeForPerformance;
            }
            
            // Адаптация под количество отверстий
            if (ShaftData.Holes.Count > MaxHolesForOptimization)
            {
                HolesAdaptationType = CreateShaftCmdAdaptationType.OptimizeForMemory;
            }
            
            // Адаптация под количество элементов
            if (ShaftData.Elements.Count > MaxElementsForOptimization)
            {
                ElementsAdaptationType = CreateShaftCmdAdaptationType.OptimizeForStorage;
            }
            
            // Адаптация под профиль производительности
            switch (PerformanceProfile)
            {
                case CreateShaftCmdPerformanceProfile.HighPerformance:
                    EnableParallelProcessing = true;
                    MaxDegreeOfParallelism = Environment.ProcessorCount;
                    break;
                case CreateShaftCmdPerformanceProfile.LowResourceUsage:
                    EnableParallelProcessing = false;
                    MaxDegreeOfParallelism = 1;
                    break;
                case CreateShaftCmdPerformanceProfile.Balanced:
                    EnableParallelProcessing = true;
                    MaxDegreeOfParallelism = Math.Min(4, Environment.ProcessorCount);
                    break;
            }
        }
        
        private List<ShaftStep> AdaptSteps(List<ShaftStep> steps)
        {
            switch (StepsAdaptationType)
            {
                case CreateShaftCmdAdaptationType.OptimizeForPerformance:
                    return OptimizeStepsForPerformance(steps);
                    
                case CreateShaftCmdAdaptationType.OptimizeForMemory:
                    return OptimizeStepsForMemory(steps);
                    
                case CreateShaftCmdAdaptationType.OptimizeForStorage:
                    return OptimizeStepsForStorage(steps);
                    
                case CreateShaftCmdAdaptationType.ApplyTarget:
                    return steps; // В реальной реализации здесь будет целевое значение
                    
                default:
                    return steps;
            }
        }
        
        private List<ShaftHole> AdaptHoles(List<ShaftHole> holes)
        {
            switch (HolesAdaptationType)
            {
                case CreateShaftCmdAdaptationType.OptimizeForPerformance:
                    return OptimizeHolesForPerformance(holes);
                    
                case CreateShaftCmdAdaptationType.OptimizeForMemory:
                    return OptimizeHolesForMemory(holes);
                    
                case CreateShaftCmdAdaptationType.OptimizeForStorage:
                    return OptimizeHolesForStorage(holes);
                    
                case CreateShaftCmdAdaptationType.ApplyTarget:
                    return holes; // В реальной реализации здесь будет целевое значение
                    
                default:
                    return holes;
            }
        }
        
        private List<Element> AdaptElements(List<Element> elements)
        {
            switch (ElementsAdaptationType)
            {
                case CreateShaftCmdAdaptationType.OptimizeForPerformance:
                    return OptimizeElementsForPerformance(elements);
                    
                case CreateShaftCmdAdaptationType.OptimizeForMemory:
                    return OptimizeElementsForMemory(elements);
                    
                case CreateShaftCmdAdaptationType.OptimizeForStorage:
                    return OptimizeElementsForStorage(elements);
                    
                case CreateShaftCmdAdaptationType.ApplyTarget:
                    return elements; // В реальной реализации здесь будет целевое значение
                    
                default:
                    return elements;
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
        
        // Оптимизация ступеней для хранения
        private List<ShaftStep> OptimizeStepsForStorage(List<ShaftStep> steps)
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
        
        // Оптимизация отверстий для хранения
        private List<ShaftHole> OptimizeHolesForStorage(List<ShaftHole> holes)
        {
            if (holes.Count > MaxHolesForOptimization)
            {
                // Оптимизация больших наборов данных
                return holes.Take(MaxHolesForOptimization).ToList();
            }
            return holes;
        }
        
        // Оптимизация элементов для производительности
        private List<Element> OptimizeElementsForPerformance(List<Element> elements)
        {
            if (elements.Count > MaxElementsForOptimization)
            {
                // Оптимизация больших наборов данных
                return elements.Take(MaxElementsForOptimization).ToList();
            }
            return elements;
        }
        
        // Оптимизация элементов для памяти
        private List<Element> OptimizeElementsForMemory(List<Element> elements)
        {
            if (elements.Count > MaxElementsForOptimization)
            {
                // Оптимизация больших наборов данных
                return elements.Take(MaxElementsForOptimization).ToList();
            }
            return elements;
        }
        
        // Оптимизация элементов для хранения
        private List<Element> OptimizeElementsForStorage(List<Element> elements)
        {
            if (elements.Count > MaxElementsForOptimization)
            {
                // Оптимизация больших наборов данных
                return elements.Take(MaxElementsForOptimization).ToList();
            }
            return elements;
        }
        
        public bool IsOptimized()
        {
            return ShaftData != null && 
                   ShaftData.Steps.Count <= MaxStepsForOptimization && 
                   ShaftData.Holes.Count <= MaxHolesForOptimization && 
                   ShaftData.Elements.Count <= MaxElementsForOptimization;
        }
        
        public void OptimizeData()
        {
            if (ShaftData != null)
            {
                ShaftData.Steps = AdaptSteps(ShaftData.Steps);
                ShaftData.Holes = AdaptHoles(ShaftData.Holes);
                ShaftData.Elements = AdaptElements(ShaftData.Elements);
            }
        }
        
        public void ClearLazyLoadedData()
        {
            LazyLoadedSteps.Clear();
            LazyLoadedHoles.Clear();
            LazyLoadedElements.Clear();
        }
        
        public void PreloadData()
        {
            if (ShaftData == null) return;
            
            // Предварительная загрузка данных
            for (int i = 0; i < ShaftData.Steps.Count; i++)
            {
                if (!LazyLoadedSteps.ContainsKey(i))
                {
                    LazyLoadedSteps[i] = ShaftData.Steps[i];
                }
            }
            
            for (int i = 0; i < ShaftData.Holes.Count; i++)
            {
                if (!LazyLoadedHoles.ContainsKey(i))
                {
                    LazyLoadedHoles[i] = ShaftData.Holes[i];
                }
            }
            
            for (int i = 0; i < ShaftData.Elements.Count; i++)
            {
                if (!LazyLoadedElements.ContainsKey(i))
                {
                    LazyLoadedElements[i] = ShaftData.Elements[i];
                }
            }
        }
        
        public void CompressData()
        {
            if (EnableDataCompression && ShouldCompress())
            {
                // Реализация сжатия данных
                LastCompressionTime = DateTime.Now;
            }
        }
        
        private bool ShouldCompress()
        {
            return DateTime.Now - LastCompressionTime > CompressionInterval;
        }
        
        public void DecompressData()
        {
            // Реализация распаковки данных
        }
        
        public bool IsDataCompressed()
        {
            return CompressedData != null && CompressedData.Length > 0;
        }
        
        public void SetPerformanceProfile(CreateShaftCmdPerformanceProfile profile)
        {
            PerformanceProfile = profile;
            AdaptToCurrentParameters();
        }
        
        public void SetResourceUsage(CreateShaftCmdResourceUsage usage)
        {
            ResourceUsage = usage;
            AdaptToCurrentParameters();
        }
        
        public void LogOperation(string operation)
        {
            Console.WriteLine($"[AdaptiveCreateShaftCmd] {operation}");
        }
    }
    
    // Адаптивная команда создания вала с контекстом
    public class ContextualCreateShaftCmd : AdaptiveCreateShaftCmd
    {
        public CreateShaftCmdContext Context { get; set; }
        public Dictionary<CreateShaftCmdContext, CreateShaftCmd> ContextCommands { get; set; } = new Dictionary<CreateShaftCmdContext, CreateShaftCmd>();
        
        public ContextualCreateShaftCmd()
        {
            Context = CreateShaftCmdContext.Default;
        }
        
        public override void Run()
        {
            if (ContextCommands.ContainsKey(Context) && ContextCommands[Context] != null)
            {
                ContextCommands[Context].Run();
            }
            else
            {
                base.Run();
            }
        }
        
        public void SetCommandForContext(CreateShaftCmdContext context, CreateShaftCmd command)
        {
            ContextCommands[context] = command;
        }
        
        public CreateShaftCmd GetCommandForContext(CreateShaftCmdContext context)
        {
            return ContextCommands.ContainsKey(context) ? ContextCommands[context] : null;
        }
        
        public void SwitchContext(CreateShaftCmdContext newContext)
        {
            Context = newContext;
        }
        
        public List<CreateShaftCmdContext> GetAvailableContexts()
        {
            return ContextCommands.Keys.ToList();
        }
    }
    
    // Адаптивная команда создания вала с историей изменений
    public class HistoricalCreateShaftCmd : ContextualCreateShaftCmd
    {
        public List<CreateShaftCmdHistory> History { get; set; } = new List<CreateShaftCmdHistory>();
        public int MaxHistorySize { get; set; } = 100;
        public bool EnableHistory { get; set; } = true;
        
        public HistoricalCreateShaftCmd()
        {
            MaxHistorySize = 100;
        }
        
        public override void Run()
        {
            if (EnableHistory)
            {
                AddToHistory();
            }
            base.Run();
        }
        
        private void AddToHistory()
        {
            var historyEntry = new CreateShaftCmdHistory
            {
                Timestamp = DateTime.Now,
                ShaftData = ShaftData != null ? new ShaftData(ShaftData) : null,
                Status = GetStatus(),
                Context = Context
            };
            
            History.Add(historyEntry);
            
            // Ограничение размера истории
            if (History.Count > MaxHistorySize)
            {
                History.RemoveAt(0);
            }
        }
        
        public List<CreateShaftCmdHistory> GetHistoryForContext(CreateShaftCmdContext context)
        {
            return History.Where(h => h.Context == context).ToList();
        }
        
        public List<CreateShaftCmdHistory> GetRecentHistory(int count)
        {
            return History.TakeLast(count).ToList();
        }
        
        public void ClearHistory()
        {
            History.Clear();
        }
        
        public void RestoreFromHistory(CreateShaftCmdHistory historyEntry)
        {
            if (historyEntry != null && historyEntry.ShaftData != null)
            {
                ShaftData = new ShaftData(historyEntry.ShaftData);
                Context = historyEntry.Context;
            }
        }
    }
}

// Контекст команды создания вала
public enum CreateShaftCmdContext
{
    Default,
    Design,
    Analysis,
    Manufacturing,
    Inspection
}

// Правила адаптации команды создания вала
public enum CreateShaftCmdAdaptationType
{
    None,
    OptimizeForPerformance,
    OptimizeForMemory,
    OptimizeForStorage,
    ApplyTarget
}

// Профиль производительности команды создания вала
public enum CreateShaftCmdPerformanceProfile
{
    HighPerformance,
    Balanced,
    LowResourceUsage
}

// Использование ресурсов команды создания вала
public enum CreateShaftCmdResourceUsage
{
    Low,
    Moderate,
    High
}

// Статус команды создания вала
public enum CreateShaftCmdStatus
{
    Idle,
    Running,
    CreatingShaft,
    ShaftCreated,
    CreatingPrimitives,
    PrimitivesCreated,
    CreatingLCS,
    LCSCreated,
    CreatingVariables,
    VariablesCreated,
    Completed,
    Cancelled,
    Error
}

// Аргументы события прогресса
public class ProgressEventArgs : EventArgs
{
    public int Progress { get; set; }
    public string Message { get; set; }
    
    public ProgressEventArgs(int progress, string message)
    {
        Progress = progress;
        Message = message;
    }
}

// Аргументы события статуса
public class StatusEventArgs : EventArgs
{
    public CreateShaftCmdStatus OldStatus { get; set; }
    public CreateShaftCmdStatus NewStatus { get; set; }
    
    public StatusEventArgs(CreateShaftCmdStatus oldStatus, CreateShaftCmdStatus newStatus)
    {
        OldStatus = oldStatus;
        NewStatus = newStatus;
    }
}
```

### 3. Создание команды создания вала с условной логикой

```csharp
// Команда создания вала с условной логикой на основе контекста
public static class ConditionalCreateShaftCmd
{
    // Условия для команды создания вала
    public static List<CreateShaftCmdCondition> Conditions { get; set; } = new List<CreateShaftCmdCondition>();
    
    // Стратегии для команды создания вала
    public static Dictionary<CreateShaftCmdOperationType, CreateShaftCmdOperationStrategy> Strategies { get; set; } 
        = new Dictionary<CreateShaftCmdOperationType, CreateShaftCmdOperationStrategy>();
    
    // Добавление условия
    public static void AddCondition(CreateShaftCmdCondition condition)
    {
        Conditions.Add(condition);
    }
    
    // Добавление стратегии
    public static void AddStrategy(CreateShaftCmdOperationType type, CreateShaftCmdOperationStrategy strategy)
    {
        Strategies[type] = strategy;
    }
    
    // Условная команда создания вала с автоматическим выбором стратегии
    public class ConditionalCreateShaftCmd : CreateShaftCmd
    {
        public CreateShaftCmdContext Context { get; set; }
        public bool EnableConditionalLogic { get; set; } = true;
        
        public ConditionalCreateShaftCmd()
        {
            Context = CreateShaftCmdContext.Default;
        }
        
        public override void Run()
        {
            if (EnableConditionalLogic)
            {
                ExecuteConditionalRun();
            }
            else
            {
                base.Run();
            }
        }
        
        public override void CreateShaft()
        {
            if (EnableConditionalLogic)
            {
                ExecuteConditionalCreateShaft();
            }
            else
            {
                base.CreateShaft();
            }
        }
        
        public override void CreatePrimitives()
        {
            if (EnableConditionalLogic)
            {
                ExecuteConditionalCreatePrimitives();
            }
            else
            {
                base.CreatePrimitives();
            }
        }
        
        public override void CreateLCS()
        {
            if (EnableConditionalLogic)
            {
                ExecuteConditionalCreateLCS();
            }
            else
            {
                base.CreateLCS();
            }
        }
        
        public override void CreateVariablesInFragment()
        {
            if (EnableConditionalLogic)
            {
                ExecuteConditionalCreateVariables();
            }
            else
            {
                base.CreateVariablesInFragment();
            }
        }
        
        private void ExecuteConditionalRun()
        {
            // Определение типа операции на основе условий
            CreateShaftCmdOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                Strategies[operationType].ExecuteRun(this);
            }
            else
            {
                // Если стратегия не найдена, используем стандартное выполнение
                base.Run();
            }
        }
        
        private void ExecuteConditionalCreateShaft()
        {
            // Определение типа операции на основе условий
            CreateShaftCmdOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                Strategies[operationType].ExecuteCreateShaft(this);
            }
            else
            {
                // Если стратегия не найдена, используем стандартное выполнение
                base.CreateShaft();
            }
        }
        
        private void ExecuteConditionalCreatePrimitives()
        {
            // Определение типа операции на основе условий
            CreateShaftCmdOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                Strategies[operationType].ExecuteCreatePrimitives(this);
            }
            else
            {
                // Если стратегия не найдена, используем стандартное выполнение
                base.CreatePrimitives();
            }
        }
        
        private void ExecuteConditionalCreateLCS()
        {
            // Определение типа операции на основе условий
            CreateShaftCmdOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                Strategies[operationType].ExecuteCreateLCS(this);
            }
            else
            {
                // Если стратегия не найдена, используем стандартное выполнение
                base.CreateLCS();
            }
        }
        
        private void ExecuteConditionalCreateVariables()
        {
            // Определение типа операции на основе условий
            CreateShaftCmdOperationType operationType = DetermineOperationType();
            
            // Получение стратегии
            if (Strategies.ContainsKey(operationType))
            {
                Strategies[operationType].ExecuteCreateVariables(this);
            }
            else
            {
                // Если стратегия не найдена, используем стандартное выполнение
                base.CreateVariablesInFragment();
            }
        }
        
        private CreateShaftCmdOperationType DetermineOperationType()
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
            return CreateShaftCmdOperationType.Standard;
        }
        
        private bool CheckCondition(CreateShaftCmdCondition condition)
        {
            switch (condition.Parameter)
            {
                case ConditionalCreateShaftCmdParameter.Context:
                    return (int)Context == condition.Value;
                case ConditionalCreateShaftCmdParameter.StepsCount:
                    return ShaftData?.Steps?.Count >= condition.Value;
                case ConditionalCreateShaftCmdParameter.HolesCount:
                    return ShaftData?.Holes?.Count >= condition.Value;
                case ConditionalCreateShaftCmdParameter.ElementsCount:
                    return ShaftData?.Elements?.Count >= condition.Value;
                default:
                    return false;
            }
        }
    }
    
    // Условная команда создания вала с множественными значениями
    public class MultiValueCreateShaftCmd : ConditionalCreateShaftCmd
    {
        public Dictionary<CreateShaftCmdContext, CreateShaftCmd> Values { get; set; } = new Dictionary<CreateShaftCmdContext, CreateShaftCmd>();
        
        public MultiValueCreateShaftCmd()
        {
            Values[CreateShaftCmdContext.Default] = new CreateShaftCmd();
        }
        
        public override void Run()
        {
            if (Values.ContainsKey(Context))
            {
                Values[Context].Run();
            }
            else
            {
                base.Run();
            }
        }
        
        public override void CreateShaft()
        {
            if (Values.ContainsKey(Context) && Values[Context] != null)
            {
                Values[Context].CreateShaft();
            }
            else
            {
                base.CreateShaft();
            }
        }
        
        public override void CreatePrimitives()
        {
            if (Values.ContainsKey(Context) && Values[Context] != null)
            {
                Values[Context].CreatePrimitives();
            }
            else
            {
                base.CreatePrimitives();
            }
        }
        
        public override void CreateLCS()
        {
            if (Values.ContainsKey(Context) && Values[Context] != null)
            {
                Values[Context].CreateLCS();
            }
            else
            {
                base.CreateLCS();
            }
        }
        
        public override void CreateVariablesInFragment()
        {
            if (Values.ContainsKey(Context) && Values[Context] != null)
            {
                Values[Context].CreateVariablesInFragment();
            }
            else
            {
                base.CreateVariablesInFragment();
            }
        }
        
        public void SetValueForContext(CreateShaftCmdContext context, CreateShaftCmd value)
        {
            Values[context] = value;
        }
        
        public CreateShaftCmd GetValueForContext(CreateShaftCmdContext context)
        {
            return Values.ContainsKey(context) ? Values[context] : null;
        }
        
        public void RemoveValueForContext(CreateShaftCmdContext context)
        {
            if (Values.ContainsKey(context))
            {
                Values.Remove(context);
            }
        }
    }
    
    // Условная команда создания вала с вычисляемыми значениями
    public class ComputedCreateShaftCmd : ConditionalCreateShaftCmd
    {
        public Func<CreateShaftCmdContext, CreateShaftCmd> CommandComputationFunction { get; set; }
        public bool EnableComputation { get; set; } = true;
        public CreateShaftCmd CachedCommand { get; set; }
        public DateTime LastComputationTime { get; set; }
        public TimeSpan CacheTimeout { get; set; } = TimeSpan.FromMinutes(5);
        
        public ComputedCreateShaftCmd()
        {
            CacheTimeout = TimeSpan.FromMinutes(5);
        }
        
        public override void Run()
        {
            if (EnableComputation && CommandComputationFunction != null)
            {
                // Проверка необходимости пересчета
                if (IsCacheExpired())
                {
                    CachedCommand = CommandComputationFunction(Context);
                    LastComputationTime = DateTime.Now;
                }
                
                if (CachedCommand != null)
                {
                    CachedCommand.Run();
                    return;
                }
            }
            
            base.Run();
        }
        
        public override void CreateShaft()
        {
            if (EnableComputation && CommandComputationFunction != null)
            {
                // Проверка необходимости пересчета
                if (IsCacheExpired())
                {
                    CachedCommand = CommandComputationFunction(Context);
                    LastComputationTime = DateTime.Now;
                }
                
                if (CachedCommand != null)
                {
                    CachedCommand.CreateShaft();
                    return;
                }
            }
            
            base.CreateShaft();
        }
        
        private bool IsCacheExpired()
        {
            return DateTime.Now - LastComputationTime > CacheTimeout;
        }
        
        public void InvalidateCache()
        {
            LastComputationTime = DateTime.MinValue;
            CachedCommand = null;
        }
        
        public void SetCommandComputationFunction(Func<CreateShaftCmdContext, CreateShaftCmd> function)
        {
            CommandComputationFunction = function;
            InvalidateCache();
        }
    }
    
    // Стандартная стратегия
    public static class StandardStrategy : CreateShaftCmdOperationStrategy
    {
        public override void ExecuteRun(ConditionalCreateShaftCmd cmd)
        {
            cmd.BaseRun();
        }
        
        public override void ExecuteCreateShaft(ConditionalCreateShaftCmd cmd)
        {
            cmd.BaseCreateShaft();
        }
        
        public override void ExecuteCreatePrimitives(ConditionalCreateShaftCmd cmd)
        {
            cmd.BaseCreatePrimitives();
        }
        
        public override void ExecuteCreateLCS(ConditionalCreateShaftCmd cmd)
        {
            cmd.BaseCreateLCS();
        }
        
        public override void ExecuteCreateVariables(ConditionalCreateShaftCmd cmd)
        {
            cmd.BaseCreateVariables();
        }
    }
    
    // Высокоточная стратегия
    public static class HighPrecisionStrategy : CreateShaftCmdOperationStrategy
    {
        public override void ExecuteRun(ConditionalCreateShaftCmd cmd)
        {
            // Выполнение с высокой точностью
            cmd.BaseRun();
        }
        
        public override void ExecuteCreateShaft(ConditionalCreateShaftCmd cmd)
        {
            // Создание вала с высокой точностью
            cmd.BaseCreateShaft();
        }
        
        public override void ExecuteCreatePrimitives(ConditionalCreateShaftCmd cmd)
        {
            // Создание примитивов с высокой точностью
            cmd.BaseCreatePrimitives();
        }
        
        public override void ExecuteCreateLCS(ConditionalCreateShaftCmd cmd)
        {
            // Создание LCS с высокой точностью
            cmd.BaseCreateLCS();
        }
        
        public override void ExecuteCreateVariables(ConditionalCreateShaftCmd cmd)
        {
            // Создание переменных с высокой точностью
            cmd.BaseCreateVariables();
        }
    }
    
    // Оптимизированная стратегия
    public static class OptimizedStrategy : CreateShaftCmdOperationStrategy
    {
        public override void ExecuteRun(ConditionalCreateShaftCmd cmd)
        {
            // Оптимизированное выполнение
            cmd.BaseRun();
        }
        
        public override void ExecuteCreateShaft(ConditionalCreateShaftCmd cmd)
        {
            // Оптимизированное создание вала
            cmd.BaseCreateShaft();
        }
        
        public override void ExecuteCreatePrimitives(ConditionalCreateShaftCmd cmd)
        {
            // Оптимизированное создание примитивов
            cmd.BaseCreatePrimitives();
        }
        
        public override void ExecuteCreateLCS(ConditionalCreateShaftCmd cmd)
        {
            // Оптимизированное создание LCS
            cmd.BaseCreateLCS();
        }
        
        public override void ExecuteCreateVariables(ConditionalCreateShaftCmd cmd)
        {
            // Оптимизированное создание переменных
            cmd.BaseCreateVariables();
        }
    }
    
    // Расширение базовой команды создания вала для условных команд
    public class ConditionalCreateShaftCmd : CreateShaftCmd
    {
        public void BaseRun()
        {
            base.Run();
        }
        
        public void BaseCreateShaft()
        {
            base.CreateShaft();
        }
        
        public void BaseCreatePrimitives()
        {
            base.CreatePrimitives();
        }
        
        public void BaseCreateLCS()
        {
            base.CreateLCS();
        }
        
        public void BaseCreateVariables()
        {
            base.CreateVariablesInFragment();
        }
    }
}

// Условие для команды создания вала
public class CreateShaftCmdCondition
{
    public ConditionalCreateShaftCmdParameter Parameter { get; set; }
    public ComparisonOperator Operator { get; set; }
    public double Value { get; set; }
    public CreateShaftCmdOperationType OperationType { get; set; }
}

public enum ConditionalCreateShaftCmdParameter
{
    Context,
    StepsCount,
    HolesCount,
    ElementsCount,
    Complexity
}

public enum CreateShaftCmdOperationType
{
    Standard,
    HighPrecision,
    Optimized,
    Debug
}

// Абстрактная стратегия для команды создания вала
public abstract class CreateShaftCmdOperationStrategy
{
    public abstract void ExecuteRun(ConditionalCreateShaftCmd cmd);
    public abstract void ExecuteCreateShaft(ConditionalCreateShaftCmd cmd);
    public abstract void ExecuteCreatePrimitives(ConditionalCreateShaftCmd cmd);
    public abstract void ExecuteCreateLCS(ConditionalCreateShaftCmd cmd);
    public abstract void ExecuteCreateVariables(ConditionalCreateShaftCmd cmd);
}
```

### 4. Создание команды создания вала с множественными конфигурациями

```csharp
// Команда создания вала с множественными конфигурациями
public static class MultiConfigurationCreateShaftCmd
{
    // Конфигурации для команды создания вала
    public static List<CreateShaftCmdConfiguration> Configurations { get; set; } = new List<CreateShaftCmdConfiguration>();
    public static int CurrentConfigurationIndex { get; set; } = 0;
    
    // Добавление конфигурации
    public static void AddConfiguration(CreateShaftCmdConfiguration config)
    {
        Configurations.Add(config);
    }
    
    // Получение текущей конфигурации
    public static CreateShaftCmdConfiguration GetCurrentConfiguration()
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
    public static CreateShaftCmdConfiguration SwitchToNextConfiguration()
    {
        if (Configurations.Count == 0)
            return null;
            
        CurrentConfigurationIndex = (CurrentConfigurationIndex + 1) % Configurations.Count;
        return GetCurrentConfiguration();
    }
    
    // Переключение на предыдущую конфигурацию
    public static CreateShaftCmdConfiguration SwitchToPreviousConfiguration()
    {
        if (Configurations.Count == 0)
            return null;
            
        CurrentConfigurationIndex = (CurrentConfigurationIndex - 1 + Configurations.Count) % Configurations.Count;
        return GetCurrentConfiguration();
    }
    
    // Получение конфигурации по индексу
    public static CreateShaftCmdConfiguration GetConfigurationByIndex(int index)
    {
        if (index >= 0 && index < Configurations.Count)
        {
            CurrentConfigurationIndex = index;
            return Configurations[index];
        }
        
        return null;
    }
    
    // Команда создания вала с множественными конфигурациями
    public class ConfigurableCreateShaftCmd : CreateShaftCmd
    {
        public Dictionary<CreateShaftCmdConfiguration, CreateShaftCmd> ConfigurationValues { get; set; } 
            = new Dictionary<CreateShaftCmdConfiguration, CreateShaftCmd>();
        public bool EnableConfigurationSwitching { get; set; } = true;
        
        public ConfigurableCreateShaftCmd()
        {
            ConfigurationValues[new CreateShaftCmdConfiguration { Name = "Default", IsDefault = true }] = new CreateShaftCmd();
        }
        
        public override void Run()
        {
            var currentConfig = MultiConfigurationCreateShaftCmd.GetCurrentConfiguration();
            if (currentConfig != null && ConfigurationValues.ContainsKey(currentConfig))
            {
                ConfigurationValues[currentConfig].Run();
            }
            else
            {
                base.Run();
            }
        }
        
        public override void CreateShaft()
        {
            var currentConfig = MultiConfigurationCreateShaftCmd.GetCurrentConfiguration();
            if (currentConfig != null && ConfigurationValues.ContainsKey(currentConfig))
            {
                ConfigurationValues[currentConfig].CreateShaft();
            }
            else
            {
                base.CreateShaft();
            }
        }
        
        public override void CreatePrimitives()
        {
            var currentConfig = MultiConfigurationCreateShaftCmd.GetCurrentConfiguration();
            if (currentConfig != null && ConfigurationValues.ContainsKey(currentConfig))
            {
                ConfigurationValues[currentConfig].CreatePrimitives();
            }
            else
            {
                base.CreatePrimitives();
            }
        }
        
        public override void CreateLCS()
        {
            var currentConfig = MultiConfigurationCreateShaftCmd.GetCurrentConfiguration();
            if (currentConfig != null && ConfigurationValues.ContainsKey(currentConfig))
            {
                ConfigurationValues[currentConfig].CreateLCS();
            }
            else
            {
                base.CreateLCS();
            }
        }
        
        public override void CreateVariablesInFragment()
        {
            var currentConfig = MultiConfigurationCreateShaftCmd.GetCurrentConfiguration();
            if (currentConfig != null && ConfigurationValues.ContainsKey(currentConfig))
            {
                ConfigurationValues[currentConfig].CreateVariablesInFragment();
            }
            else
            {
                base.CreateVariablesInFragment();
            }
        }
        
        public void SetValueForConfiguration(CreateShaftCmdConfiguration config, CreateShaftCmd value)
        {
            ConfigurationValues[config] = value;
        }
        
        public CreateShaftCmd GetValueForConfiguration(CreateShaftCmdConfiguration config)
        {
            return ConfigurationValues.ContainsKey(config) ? ConfigurationValues[config] : null;
        }
        
        public void RemoveConfigurationValue(CreateShaftCmdConfiguration config)
        {
            if (ConfigurationValues.ContainsKey(config))
            {
                ConfigurationValues.Remove(config);
            }
        }
        
        public List<CreateShaftCmdConfiguration> GetConfigurationsWithValues()
        {
            return ConfigurationValues.Keys.ToList();
        }
    }
    
    // Команда создания вала с режимами работы
    public class ModeCreateShaftCmd : ConfigurableCreateShaftCmd
    {
        public CreateShaftCmdMode CurrentMode { get; set; } = CreateShaftCmdMode.Standard;
        public Dictionary<CreateShaftCmdMode, CreateShaftCmd> ModeValues { get; set; } = new Dictionary<CreateShaftCmdMode, CreateShaftCmd>();
        
        public ModeCreateShaftCmd()
        {
            ModeValues[CreateShaftCmdMode.Standard] = new CreateShaftCmd();
        }
        
        public override void Run()
        {
            if (ModeValues.ContainsKey(CurrentMode))
            {
                ModeValues[CurrentMode].Run();
            }
            else
            {
                base.Run();
            }
        }
        
        public override void CreateShaft()
        {
            if (ModeValues.ContainsKey(CurrentMode) && ModeValues[CurrentMode] != null)
            {
                ModeValues[CurrentMode].CreateShaft();
            }
            else
            {
                base.CreateShaft();
            }
        }
        
        public override void CreatePrimitives()
        {
            if (ModeValues.ContainsKey(CurrentMode) && ModeValues[CurrentMode] != null)
            {
                ModeValues[CurrentMode].CreatePrimitives();
            }
            else
            {
                base.CreatePrimitives();
            }
        }
        
        public override void CreateLCS()
        {
            if (ModeValues.ContainsKey(CurrentMode) && ModeValues[CurrentMode] != null)
            {
                ModeValues[CurrentMode].CreateLCS();
            }
            else
            {
                base.CreateLCS();
            }
        }
        
        public override void CreateVariablesInFragment()
        {
            if (ModeValues.ContainsKey(CurrentMode) && ModeValues[CurrentMode] != null)
            {
                ModeValues[CurrentMode].CreateVariablesInFragment();
            }
            else
            {
                base.CreateVariablesInFragment();
            }
        }
        
        public void SetValueForMode(CreateShaftCmdMode mode, CreateShaftCmd value)
        {
            ModeValues[mode] = value;
        }
        
        public CreateShaftCmd GetValueForMode(CreateShaftCmdMode mode)
        {
            return ModeValues.ContainsKey(mode) ? ModeValues[mode] : null;
        }
        
        public void SwitchMode(CreateShaftCmdMode newMode)
        {
            CurrentMode = newMode;
        }
        
        public List<CreateShaftCmdMode> GetAvailableModes()
        {
            return ModeValues.Keys.ToList();
        }
    }
    
    // Команда создания вала с профилями
    public class ProfileCreateShaftCmd : ModeCreateShaftCmd
    {
        public string CurrentProfile { get; set; } = "Default";
        public Dictionary<string, CreateShaftCmd> ProfileValues { get; set; } = new Dictionary<string, CreateShaftCmd>();
        
        public ProfileCreateShaftCmd()
        {
            ProfileValues["Default"] = new CreateShaftCmd();
        }
        
        public override void Run()
        {
            if (ProfileValues.ContainsKey(CurrentProfile))
            {
                ProfileValues[CurrentProfile].Run();
            }
            else
            {
                base.Run();
            }
        }
        
        public override void CreateShaft()
        {
            if (ProfileValues.ContainsKey(CurrentProfile) && ProfileValues[CurrentProfile] != null)
            {
                ProfileValues[CurrentProfile].CreateShaft();
            }
            else
            {
                base.CreateShaft();
            }
        }
        
        public override void CreatePrimitives()
        {
            if (ProfileValues.ContainsKey(CurrentProfile) && ProfileValues[CurrentProfile] != null)
            {
                ProfileValues[CurrentProfile].CreatePrimitives();
            }
            else
            {
                base.CreatePrimitives();
            }
        }
        
        public override void CreateLCS()
        {
            if (ProfileValues.ContainsKey(CurrentProfile) && ProfileValues[CurrentProfile] != null)
            {
                ProfileValues[CurrentProfile].CreateLCS();
            }
            else
            {
                base.CreateLCS();
            }
        }
        
        public override void CreateVariablesInFragment()
        {
            if (ProfileValues.ContainsKey(CurrentProfile) && ProfileValues[CurrentProfile] != null)
            {
                ProfileValues[CurrentProfile].CreateVariablesInFragment();
            }
            else
            {
                base.CreateVariablesInFragment();
            }
        }
        
        public void SetValueForProfile(string profile, CreateShaftCmd value)
        {
            ProfileValues[profile] = value;
        }
        
        public CreateShaftCmd GetValueForProfile(string profile)
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
        
        public void AddProfile(string profile, CreateShaftCmd value)
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

// Конфигурация команды создания вала
public class CreateShaftCmdConfiguration
{
    public string Name { get; set; }
    public string Description { get; set; }
    public bool IsDefault { get; set; } = false;
    public CreateShaftCmdSettings Settings { get; set; }
    public CreateShaftCmdOptimizationLevel OptimizationLevel { get; set; }
    
    public CreateShaftCmdConfiguration()
    {
        Settings = new CreateShaftCmdSettings();
    }
}

// Настройки команды создания вала
public class CreateShaftCmdSettings
{
    public int MinSteps { get; set; } = 1;
    public int MaxSteps { get; set; } = 1000;
    public int MinHoles { get; set; } = 0;
    public int MaxHoles { get; set; } = 1000;
    public int MinElements { get; set; } = 0;
    public int MaxElements { get; set; } = 1000;
    public bool EnableLogging { get; set; } = true;
    public bool EnableValidation { get; set; } = true;
}

public enum CreateShaftCmdOptimizationLevel
{
    None,
    Basic,
    Advanced,
    Maximum
}

// Режимы команды создания вала
public enum CreateShaftCmdMode
{
    Standard,
    HighPrecision,
    Optimized,
    Debug
}

// Пример использования множественных конфигураций команды создания вала
public static void UseMultiConfigurationCreateShaftCmd()
{
    // Конфигурация 1: Стандартная
    CreateShaftCmdConfiguration config1 = new CreateShaftCmdConfiguration();
    config1.Name = "Стандартная конфигурация";
    config1.Description = "Стандартные настройки команды создания вала";
    config1.IsDefault = true;
    config1.Settings.EnableLogging = true;
    config1.Settings.EnableValidation = true;
    config1.OptimizationLevel = CreateShaftCmdOptimizationLevel.Basic;
    MultiConfigurationCreateShaftCmd.AddConfiguration(config1);
    
    // Конфигурация 2: Оптимизированная
    CreateShaftCmdConfiguration config2 = new CreateShaftCmdConfiguration();
    config2.Name = "Оптимизированная конфигурация";
    config2.Description = "Оптимизированные настройки команды создания вала";
    config2.Settings.EnableLogging = false;
    config2.Settings.EnableValidation = true;
    config2.OptimizationLevel = CreateShaftCmdOptimizationLevel.Advanced;
    MultiConfigurationCreateShaftCmd.AddConfiguration(config2);
    
    // Конфигурация 3: Отладочная
    CreateShaftCmdConfiguration config3 = new CreateShaftCmdConfiguration();
    config3.Name = "Отладочная конфигурация";
    config3.Description = "Настройки команды создания вала для отладки";
    config3.Settings.EnableLogging = true;
    config3.Settings.EnableValidation = true;
    config3.OptimizationLevel = CreateShaftCmdOptimizationLevel.None;
    MultiConfigurationCreateShaftCmd.AddConfiguration(config3);
    
    Console.WriteLine("Множественные конфигурации команды создания вала настроены");
}
```

## Практические рекомендации

1. Используйте параметризованную команду создания вала для создания гибких решений
2. При создании адаптивной команды создания вала учитывайте контекст использования
3. Используйте условную команду создания вала для автоматического выбора стратегии выполнения
4. При создании команды создания вала с множественными конфигурациями реализуйте систему переключения
5. Реализуйте проверки ограничений при установке значений команды создания вала
6. Используйте логирование для отслеживания изменений команды создания вала
7. При работе с множественными конфигурациями реализуйте систему описаний
8. Учитывайте ограничения T-Flex CAD API при создании команды создания вала
9. Реализуйте обработку ошибок для повышения надежности команды создания вала
10. Используйте стратегии для реализации различных подходов к работе с командой создания вала