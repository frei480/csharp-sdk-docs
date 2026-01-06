# CreateShaftCmd в T-Flex CAD API

## Описание
CreateShaftCmd - это класс команды для создания вала в T-Flex CAD API. Он реализует интерфейс ICommand и отвечает за создание 3D модели вала на основе заданных параметров.

## Основные методы
- Run() - Основной метод выполнения команды
- CreateShaft() - Создание вала
- CreatePrimitives() - Создание примитивов
- CreateLCS() - Создание локальных систем координат
- CreateVariablesInFragment() - Создание переменных во фрагменте

## Примеры использования

### 1. Базовое использование команды CreateShaftCmd

```csharp
// Создание и выполнение команды создания вала
public void CreateSimpleShaft()
{
    // Создание команды
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    // Установка параметров команды (если необходимо)
    // cmd.SomeProperty = someValue;
    
    // Выполнение команды
    cmd.Run();
}

// Создание команды с заданными параметрами
public void CreateShaftWithParameters(ShaftData shaftData)
{
    // Создание команды
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    // Передача данных вала в команду (если предусмотрено API)
    // cmd.ShaftData = shaftData;
    
    // Выполнение команды
    cmd.Run();
}
```

### 2. Создание вала с использованием CreateShaft метода

```csharp
// Создание вала с заданными параметрами
public ModelObject CreateShaftModel(Document doc, ShaftData data)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    // Создание фрагмента для вала
    Fragment3D fragment = doc.CreateFragment("Вал");
    
    // Создание вала
    ModelObject shaftModel = cmd.CreateShaft(doc, fragment, data);
    
    return shaftModel;
}

// Создание вала с пользовательскими параметрами
public ModelObject CreateCustomShaft(Document doc, List<ShaftStep> steps, List<ShaftHole> holes)
{
    // Создание данных вала
    ShaftData data = new ShaftData();
    data.Steps = new List<ShaftStep>(steps);
    data.Holes = new List<ShaftHole>(holes);
    data.Name = "Пользовательский вал";
    data.Material = "Сталь 45";
    
    // Создание команды и вала
    CreateShaftCmd cmd = new CreateShaftCmd();
    Fragment3D fragment = doc.CreateFragment("Пользовательский вал");
    ModelObject shaftModel = cmd.CreateShaft(doc, fragment, data);
    
    return shaftModel;
}
```

### 3. Создание примитивов вала

```csharp
// Создание примитивов для ступеней вала
public List<ModelObject> CreateShaftPrimitives(Document doc, Fragment3D fragment, ShaftData data)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    // Создание списка для хранения примитивов
    List<ModelObject> primitives = new List<ModelObject>();
    
    // Создание примитивов для каждой ступени
    for (int i = 0; i < data.Steps.Count; i++)
    {
        ModelObject primitive = cmd.CreatePrimitives(doc, fragment, data.Steps[i], i);
        if (primitive != null)
        {
            primitives.Add(primitive);
        }
    }
    
    return primitives;
}

// Создание примитива для отдельной ступени
public ModelObject CreateStepPrimitive(Document doc, Fragment3D fragment, ShaftStep step, int index)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    return cmd.CreatePrimitives(doc, fragment, step, index);
}
```

### 4. Создание локальных систем координат

```csharp
// Создание локальных систем координат для ступеней
public List<LocalCoordinateSystem> CreateLCSForSteps(Document doc, Fragment3D fragment, ShaftData data)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    // Создание списка для хранения LCS
    List<LocalCoordinateSystem> lcsList = new List<LocalCoordinateSystem>();
    
    // Создание LCS для каждой ступени
    for (int i = 0; i < data.Steps.Count; i++)
    {
        LocalCoordinateSystem lcs = cmd.CreateLCS(doc, fragment, data.Steps, i);
        if (lcs != null)
        {
            lcsList.Add(lcs);
        }
    }
    
    return lcsList;
}

// Создание LCS для отдельной ступени
public LocalCoordinateSystem CreateStepLCS(Document doc, Fragment3D fragment, List<ShaftStep> steps, int index)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    return cmd.CreateLCS(doc, fragment, steps, index);
}
```

### 5. Работа с переменными во фрагменте

```csharp
// Создание переменных для ступени во фрагменте
public void CreateVariablesForStep(Fragment3D fragment, ShaftStep step, int index)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    // Создание переменных для примитива ступени
    switch (step.PrimitiveType)
    {
        case PrimitiveType.Cylinder:
            cmd.CreateVariablesInFragment(fragment, step.PrimitiveCylinder, index);
            break;
        case PrimitiveType.Cone:
            cmd.CreateVariablesInFragment(fragment, step.PrimitiveCone, index);
            break;
        case PrimitiveType.Prisma:
            cmd.CreateVariablesInFragment(fragment, step.PrimitivePrisma, index);
            break;
    }
}

// Создание переменных для всех ступеней
public void CreateVariablesForAllSteps(Fragment3D fragment, ShaftData data)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    for (int i = 0; i < data.Steps.Count; i++)
    {
        var step = data.Steps[i];
        
        // Создание переменных для примитива ступени
        switch (step.PrimitiveType)
        {
            case PrimitiveType.Cylinder:
                cmd.CreateVariablesInFragment(fragment, step.PrimitiveCylinder, i);
                break;
            case PrimitiveType.Cone:
                cmd.CreateVariablesInFragment(fragment, step.PrimitiveCone, i);
                break;
            case PrimitiveType.Prisma:
                cmd.CreateVariablesInFragment(fragment, step.PrimitivePrisma, i);
                break;
        }
        
        // Создание переменных для элементов кромок
        cmd.CreateVariablesInFragment(fragment, step.EdgeFirst, i, 1);
        cmd.CreateVariablesInFragment(fragment, step.EdgeSecond, i, 2);
    }
}
```

### 6. Расширенные примеры использования

```csharp
// Создание вала с последующей настройкой отображения
public ModelObject CreateShaftWithDisplaySettings(Document doc, ShaftData data)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    // Создание фрагмента
    Fragment3D fragment = doc.CreateFragment(data.Name);
    
    // Создание вала
    ModelObject shaftModel = cmd.CreateShaft(doc, fragment, data);
    
    // Настройка отображения (если необходимо)
    if (shaftModel != null)
    {
        // Установка прозрачности
        Utils.SetModelObjectTransparency(shaftModel, 0); // Непрозрачный
        
        // Скрытие модели (если необходимо)
        // Utils.HideModelObject(shaftModel);
    }
    
    return shaftModel;
}

// Создание вала с обработкой ошибок
public ModelObject CreateShaftWithErrorHandling(Document doc, ShaftData data)
{
    try
    {
        CreateShaftCmd cmd = new CreateShaftCmd();
        
        // Проверка входных данных
        if (doc == null || data == null || data.Steps.Count == 0)
        {
            throw new ArgumentException("Некорректные входные данные");
        }
        
        // Создание фрагмента
        Fragment3D fragment = doc.CreateFragment(data.Name);
        
        // Создание вала
        ModelObject shaftModel = cmd.CreateShaft(doc, fragment, data);
        
        // Проверка результата
        if (shaftModel == null)
        {
            throw new InvalidOperationException("Не удалось создать вал");
        }
        
        return shaftModel;
    }
    catch (Exception ex)
    {
        // Логирование ошибки
        Console.WriteLine($"Ошибка при создании вала: {ex.Message}");
        return null;
    }
}

// Создание вала с последующей регенерацией документа
public ModelObject CreateShaftWithRegeneration(Document doc, ShaftData data)
{
    CreateShaftCmd cmd = new CreateShaftCmd();
    
    // Создание фрагмента
    Fragment3D fragment = doc.CreateFragment(data.Name);
    
    // Создание вала
    ModelObject shaftModel = cmd.CreateShaft(doc, fragment, data);
    
    // Регенерация документа
    if (shaftModel != null)
    {
        Utils.RegenerateDoc(doc);
    }
    
    return shaftModel;
}
```

## Практические рекомендации

1. Всегда создавайте фрагмент перед вызовом метода CreateShaft
2. Используйте метод Run() для выполнения команды в стандартном режиме
3. При создании примитивов учитывайте тип примитива ступени
4. При работе с переменными используйте индекс ступени для правильной идентификации
5. После создания вала рекомендуется выполнить регенерацию документа
6. Обрабатывайте возможные ошибки при создании вала
7. Используйте вспомогательные методы класса Utils для настройки отображения
8. При создании сложных валов разбивайте процесс на этапы (примитивы, LCS, переменные)
9. Проверяйте корректность входных данных перед созданием вала
10. Используйте осмысленные имена для фрагментов и моделей