# Шпаргалка CreateShaftCmd T-Flex CAD API

## Основная информация

**Класс:** CreateShaftCmd
**Пространство имен:** TFlex.Shaft.Plugin.Commands
**Тип:** Команда создания вала
**Назначение:** Реализует команду создания трехмерной модели вала в T-Flex CAD

## Основные свойства

| Свойство | Тип | Описание | Использование |
|----------|-----|----------|---------------|
| ShaftData | ShaftData | Данные вала | Хранит информацию о параметрах вала |
| Document | Document | Документ T-Flex | Ссылка на текущий документ CAD |
| Model | Model3D | Трехмерная модель | Ссылка на создаваемую 3D модель |
| Fragments | List<Fragment3D> | Фрагменты модели | Список фрагментов трехмерной модели |
| Variables | Dictionary<string, Variable> | Переменные модели | Словарь параметрических переменных |
| IsPreview | bool | Режим предпросмотра | Флаг режима предварительного просмотра |
| Progress | int | Прогресс выполнения | Текущий прогресс выполнения команды |
| TotalSteps | int | Общее количество шагов | Общее количество шагов выполнения |

## Основные методы

### Конструкторы

#### CreateShaftCmd()
**Описание:** Создает новый экземпляр CreateShaftCmd
**Параметры:** Нет
**Использование:** Инициализация команды создания вала

#### CreateShaftCmd(ShaftData data)
**Описание:** Создает новый экземпляр CreateShaftCmd с указанными данными
**Параметры:** data (ShaftData) - данные вала
**Использование:** Создание команды с готовыми данными

### Методы создания вала

#### CreateShaft(ShaftData data)
**Возвращаемый тип:** bool
**Описание:** Создает трехмерную модель вала из данных
**Параметры:** data (ShaftData) - данные вала
**Использование:** Основной метод создания вала

#### CreatePreview(ShaftData data)
**Возвращаемый тип:** bool
**Описание:** Создает предварительный просмотр вала
**Параметры:** data (ShaftData) - данные вала
**Использование:** Создание предварительного просмотра

#### CreatePrimitives(List<ShaftStep> steps)
**Возвращаемый тип:** List<ModelObject>
**Описание:** Создает примитивы для ступеней вала
**Параметры:** steps (List<ShaftStep>) - список ступеней
**Использование:** Создание геометрических примитивов

#### CreateLCS(List<ShaftStep> steps)
**Возвращаемый тип:** List<LCS>
**Описание:** Создает локальные координатные системы для ступеней
**Параметры:** steps (List<ShaftStep>) - список ступеней
**Использование:** Создание систем координат для ступеней

#### CreateVariablesInFragment(Fragment3D fragment, ShaftStep step, int index)
**Возвращаемый тип:** void
**Описание:** Создает переменные в фрагменте для ступени
**Параметры:** 
- fragment (Fragment3D) - фрагмент модели
- step (ShaftStep) - ступень вала
- index (int) - индекс ступени
**Использование:** Создание параметрических переменных

### Методы управления моделью

#### AddStepToModel(ShaftStep step, LCS lcs)
**Возвращаемый тип:** ModelObject
**Описание:** Добавляет ступень в модель
**Параметры:** 
- step (ShaftStep) - ступень вала
- lcs (LCS) - локальная координатная система
**Использование:** Добавление ступени в трехмерную модель

#### AddHoleToModel(ShaftHole hole, ModelObject target)
**Возвращаемый тип:** bool
**Описание:** Добавляет отверстие в модель
**Параметры:** 
- hole (ShaftHole) - отверстие вала
- target (ModelObject) - целевой объект для отверстия
**Использование:** Добавление отверстия в модель

#### ApplyEdgeTreatment(ElementEdge edge, ModelObject target)
**Возвращаемый тип:** bool
**Описание:** Применяет обработку кромки к объекту
**Параметры:** 
- edge (ElementEdge) - обработка кромки
- target (ModelObject) - целевой объект
**Использование:** Применение радиусов и фасок

#### ApplyElement(Element element, ModelObject target)
**Возвращаемый тип:** bool
**Описание:** Применяет элемент к объекту
**Параметры:** 
- element (Element) - элемент вала
- target (ModelObject) - целевой объект
**Использование:** Применение ключей, колец и других элементов

### Методы управления документом

#### InitializeDocument()
**Возвращаемый тип:** bool
**Описание:** Инициализирует документ для создания вала
**Параметры:** Нет
**Использование:** Подготовка документа к созданию модели

#### FinalizeDocument()
**Возвращаемый тип:** bool
**Описание:** Завершает работу с документом
**Параметры:** Нет
**Использование:** Завершение создания модели

#### RegenerateModel()
**Возвращаемый тип:** bool
**Описание:** Регенерирует модель
**Параметры:** Нет
**Использование:** Обновление отображения модели

### Методы управления прогрессом

#### UpdateProgress(int current, int total)
**Возвращаемый тип:** void
**Описание:** Обновляет прогресс выполнения
**Параметры:** 
- current (int) - текущий шаг
- total (int) - общее количество шагов
**Использование:** Обновление индикатора прогресса

#### ReportError(string message)
**Возвращаемый тип:** void
**Описание:** Сообщает об ошибке
**Параметры:** message (string) - сообщение об ошибке
**Использование:** Отчет об ошибках выполнения

## Примеры использования

### Создание команды и инициализация

```csharp
// Создание команды создания вала
CreateShaftCmd createCmd = new CreateShaftCmd();

// Создание данных вала
ShaftData shaftData = new ShaftData();
shaftData.Name = "Тестовый вал";
shaftData.Material = "Сталь 45";

// Добавление ступеней
ShaftStep step1 = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
step1.Name = "Основная ступень";
shaftData.AddStep(step1);

ShaftStep step2 = new ShaftStep(PrimitiveType.Cylinder, 30.0, 80.0);
step2.Name = "Хвостовик";
shaftData.AddStep(step2);

// Инициализация команды с данными
createCmd.ShaftData = shaftData;
```

### Создание вала из данных

```csharp
// Создание команды
CreateShaftCmd createCmd = new CreateShaftCmd();

// Создание данных вала
ShaftData shaftData = CreateSampleShaftData();

// Создание вала
bool success = createCmd.CreateShaft(shaftData);

if (success)
{
    Console.WriteLine("Вал успешно создан");
}
else
{
    Console.WriteLine("Ошибка создания вала");
}

// Вспомогательный метод для создания данных
private static ShaftData CreateSampleShaftData()
{
    ShaftData data = new ShaftData();
    data.Name = "Образец вала";
    data.Material = "Сталь 45";
    
    // Основная ступень
    ShaftStep mainStep = new ShaftStep(PrimitiveType.Cylinder, 50.0, 150.0);
    mainStep.Name = "Основная ступень";
    
    // Добавление обработок кромок
    ElementEdge startEdge = new ElementEdge();
    startEdge.SetRadius(2.0, EdgePosition.Start);
    mainStep.AddEdge(startEdge);
    
    ElementEdge endEdge = new ElementEdge();
    endEdge.SetRadius(2.0, EdgePosition.End);
    mainStep.AddEdge(endEdge);
    
    data.AddStep(mainStep);
    
    // Хвостовик
    ShaftStep stubStep = new ShaftStep(PrimitiveType.Cylinder, 30.0, 100.0);
    stubStep.Name = "Хвостовик";
    data.AddStep(stubStep);
    
    return data;
}
```

### Создание предварительного просмотра

```csharp
// Создание команды
CreateShaftCmd previewCmd = new CreateShaftCmd();
previewCmd.IsPreview = true; // Включить режим предпросмотра

// Создание данных вала
ShaftData shaftData = CreateSampleShaftData();

// Создание предварительного просмотра
bool previewSuccess = previewCmd.CreatePreview(shaftData);

if (previewSuccess)
{
    Console.WriteLine("Предварительный просмотр создан");
}
else
{
    Console.WriteLine("Ошибка создания предварительного просмотра");
}

// Обновление предварительного просмотра при изменении данных
private static void UpdatePreview(CreateShaftCmd cmd, ShaftData newData)
{
    // Очистка предыдущего предварительного просмотра
    ClearPreview(cmd);
    
    // Создание нового предварительного просмотра
    cmd.CreatePreview(newData);
    
    Console.WriteLine("Предварительный просмотр обновлен");
}

private static void ClearPreview(CreateShaftCmd cmd)
{
    // Удаление объектов предварительного просмотра
    if (cmd.Model != null)
    {
        // Удаление объектов модели
        cmd.Model.Clear();
    }
    
    Console.WriteLine("Предварительный просмотр очищен");
}
```

### Работа с примитивами и координатными системами

```csharp
// Создание команды
CreateShaftCmd createCmd = new CreateShaftCmd();

// Создание данных ступеней
List<ShaftStep> steps = new List<ShaftStep>();
ShaftStep step1 = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
ShaftStep step2 = new ShaftStep(PrimitiveType.Cone, 50.0, 30.0, 50.0);
ShaftStep step3 = new ShaftStep(PrimitiveType.Cylinder, 30.0, 80.0);

steps.Add(step1);
steps.Add(step2);
steps.Add(step3);

// Создание примитивов
List<ModelObject> primitives = createCmd.CreatePrimitives(steps);

// Создание локальных координатных систем
List<LCS> lcsList = createCmd.CreateLCS(steps);

Console.WriteLine($"Создано примитивов: {primitives.Count}");
Console.WriteLine($"Создано систем координат: {lcsList.Count}");
```

### Работа с переменными модели

```csharp
// Создание команды
CreateShaftCmd createCmd = new CreateShaftCmd();

// Создание фрагмента (в реальном коде получается из документа)
Fragment3D fragment = new Fragment3D(); // Упрощенный пример

// Создание ступени
ShaftStep step = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
step.Name = "Основная ступень";

// Создание переменных в фрагменте
createCmd.CreateVariablesInFragment(fragment, step, 0);

// Пример работы с переменными
private static void WorkWithVariables(CreateShaftCmd cmd, ShaftData data)
{
    // Создание фрагментов для каждой ступени
    for (int i = 0; i < data.Steps.Count; i++)
    {
        Fragment3D fragment = new Fragment3D(); // Упрощенный пример
        cmd.CreateVariablesInFragment(fragment, data.Steps[i], i);
    }
    
    Console.WriteLine("Переменные созданы для всех ступеней");
}
```

## Практические рекомендации

### Рекомендации по использованию

1. **Используйте команду в контексте T-Flex CAD**
   - Команда должна выполняться в контексте активного документа T-Flex CAD
   - Убедитесь, что доступны все необходимые API компоненты

2. **Проверяйте данные перед созданием вала**
   - Всегда проверяйте валидность ShaftData перед вызовом CreateShaft
   - Это помогает избежать ошибок во время выполнения

3. **Используйте режим предпросмотра для тестирования**
   - Используйте CreatePreview для быстрого предварительного просмотра
   - Это экономит время при тестировании различных конфигураций

4. **Управляйте прогрессом выполнения**
   - Используйте UpdateProgress для отображения прогресса создания вала
   - Это улучшает пользовательский опыт при создании сложных моделей

### Антипаттерны

1. **Не вызывайте команду вне контекста T-Flex CAD**
   - Команда требует наличия активного документа и API
   - Не пытайтесь выполнить команду без необходимой инфраструктуры

2. **Не игнорируйте ошибки выполнения**
   - Всегда проверяйте возвращаемые значения методов
   - Используйте ReportError для сообщения об ошибках

3. **Не создавайте дублирующие объекты**
   - Проверяйте наличие объектов перед созданием
   - Используйте существующие фрагменты и переменные при возможности

## Распространенные ошибки

### Ошибка 1: Вызов команды без активного документа

```csharp
// Неправильно
CreateShaftCmd cmd = new CreateShaftCmd();
ShaftData data = CreateSampleData();
bool result = cmd.CreateShaft(data); // Ошибка: нет активного документа

// Правильно
CreateShaftCmd cmd = new CreateShaftCmd();
cmd.Document = GetActiveDocument(); // Установка активного документа
ShaftData data = CreateSampleData();
bool result = cmd.CreateShaft(data);
```

### Ошибка 2: Игнорирование валидации данных

```csharp
// Неправильно
CreateShaftCmd cmd = new CreateShaftCmd();
ShaftData invalidData = new ShaftData(); // Невалидные данные
cmd.CreateShaft(invalidData); // Ошибка: невалидные данные

// Правильно
CreateShaftCmd cmd = new CreateShaftCmd();
ShaftData data = CreateSampleData();

if (data.Validate())
{
    cmd.CreateShaft(data);
}
else
{
    Console.WriteLine("Невалидные данные вала");
}
```

## Лучшие практики

### 1. Использование фабричного метода для создания команд

```csharp
public static class CreateShaftCmdFactory
{
    public static CreateShaftCmd CreateForDocument(Document document)
    {
        CreateShaftCmd cmd = new CreateShaftCmd();
        cmd.Document = document;
        return cmd;
    }
    
    public static CreateShaftCmd CreateForPreview(Document document)
    {
        CreateShaftCmd cmd = CreateForDocument(document);
        cmd.IsPreview = true;
        return cmd;
    }
    
    public static CreateShaftCmd CreateWithProgress(Document document, IProgressReporter reporter)
    {
        CreateShaftCmd cmd = CreateForDocument(document);
        // Установка обработчика прогресса
        return cmd;
    }
}

// Использование
Document activeDoc = GetActiveDocument();
CreateShaftCmd cmd = CreateShaftCmdFactory.CreateForDocument(activeDoc);
CreateShaftCmd previewCmd = CreateShaftCmdFactory.CreateForPreview(activeDoc);
```

### 2. Обработка ошибок и исключений

```csharp
public static class CreateShaftCmdExtensions
{
    public static bool SafeCreateShaft(this CreateShaftCmd cmd, ShaftData data, out string errorMessage)
    {
        errorMessage = string.Empty;
        
        try
        {
            // Проверка данных
            if (!data.Validate())
            {
                errorMessage = "Невалидные данные вала";
                return false;
            }
            
            // Проверка документа
            if (cmd.Document == null)
            {
                errorMessage = "Не задан документ T-Flex CAD";
                return false;
            }
            
            // Создание вала
            bool result = cmd.CreateShaft(data);
            
            if (!result)
            {
                errorMessage = "Ошибка создания вала";
            }
            
            return result;
        }
        catch (Exception ex)
        {
            errorMessage = $"Исключение при создании вала: {ex.Message}";
            return false;
        }
    }
}

// Использование
CreateShaftCmd cmd = new CreateShaftCmd();
ShaftData data = CreateSampleData();
string error;

if (cmd.SafeCreateShaft(data, out error))
{
    Console.WriteLine("Вал успешно создан");
}
else
{
    Console.WriteLine($"Ошибка: {error}");
}
```

### 3. Создание шаблонов команд

```csharp
public static class CreateShaftCmdTemplates
{
    public static CreateShaftCmd CreateStandardShaftCommand(Document document)
    {
        CreateShaftCmd cmd = new CreateShaftCmd();
        cmd.Document = document;
        return cmd;
    }
    
    public static CreateShaftCmd CreatePreviewCommand(Document document)
    {
        CreateShaftCmd cmd = CreateStandardShaftCommand(document);
        cmd.IsPreview = true;
        return cmd;
    }
    
    public static CreateShaftCmd CreateBatchCommand(Document document)
    {
        CreateShaftCmd cmd = CreateStandardShaftCommand(document);
        // Настройка для пакетной обработки
        return cmd;
    }
    
    public static CreateShaftCmd CreateOptimizedCommand(Document document)
    {
        CreateShaftCmd cmd = CreateStandardShaftCommand(document);
        // Настройка для оптимизированного создания
        return cmd;
    }
}

// Использование
Document doc = GetActiveDocument();
CreateShaftCmd standardCmd = CreateShaftCmdTemplates.CreateStandardShaftCommand(doc);
CreateShaftCmd previewCmd = CreateShaftCmdTemplates.CreatePreviewCommand(doc);
```

## Интеграция с другими компонентами

### ShaftData

CreateShaftCmd использует ShaftData для получения параметров вала перед созданием геометрии.

### Document

CreateShaftCmd использует Document для создания и управления трехмерной моделью.

### Model3D

CreateShaftCmd создает и управляет объектами Model3D при создании вала.

### Fragment3D

CreateShaftCmd использует Fragment3D для создания параметрических фрагментов модели.

### ShaftStep

CreateShaftCmd использует ShaftStep для создания геометрических примитивов ступеней.

### ShaftHole

CreateShaftCmd использует ShaftHole для создания отверстий в модели вала.

## Сериализация

### XML сериализация команды

```csharp
// Пример XML представления команды (упрощенное представление)
/*
<CreateShaftCmd>
    <IsPreview>false</IsPreview>
    <Progress>0</Progress>
    <TotalSteps>0</TotalSteps>
    <ShaftData>
        <Name>Тестовый вал</Name>
        <Material>Сталь 45</Material>
        <Steps>
            <ShaftStep>
                <Type>Cylinder</Type>
                <Diameter>50.0</Diameter>
                <Length>100.0</Length>
            </ShaftStep>
        </Steps>
    </ShaftData>
</CreateShaftCmd>
*/
```

## Тестирование

### Основные сценарии тестирования

1. **Проверка создания команды**
   - Создание команды без параметров
   - Создание команды с данными вала

2. **Проверка создания вала**
   - Создание вала из корректных данных
   - Создание вала из некорректных данных
   - Создание вала без активного документа

3. **Проверка предварительного просмотра**
   - Создание предварительного просмотра
   - Обновление предварительного просмотра
   - Очистка предварительного просмотра

4. **Проверка работы с примитивами**
   - Создание примитивов для ступеней
   - Создание локальных координатных систем
   - Создание переменных в фрагментах

5. **Проверка обработки ошибок**
   - Обработка ошибок валидации данных
   - Обработка ошибок создания модели
   - Обработка исключений

## Производительность

### Рекомендации по оптимизации

1. **Используйте кэширование для повторяющихся операций**
   - Кэшируйте созданные примитивы и системы координат
   - Используйте повторное использование фрагментов

2. **Минимизируйте количество операций с документом**
   - Группируйте операции создания объектов
   - Минимизируйте количество регенераций модели

3. **Используйте асинхронную обработку для сложных операций**
   - Выполняйте создание сложных моделей асинхронно
   - Обновляйте прогресс выполнения

## Совместимость

### Обратная совместимость

1. **Добавление новых свойств**
   - Добавление новых свойств не нарушает совместимость
   - Существующий код продолжает работать

2. **Изменение существующих свойств**
   - Изменение типов существующих свойств нарушает совместимость
   - Требует обновления существующего кода

## Дополнительные ресурсы

### См. также

- ShaftData - класс данных вала
- Document - класс документа T-Flex CAD
- Model3D - класс трехмерной модели
- Fragment3D - класс фрагмента трехмерной модели
- ShaftStep - класс ступени вала
- ShaftHole - класс отверстия в валу

### Примеры в коде

```csharp
// Полный пример использования CreateShaftCmd
public class CreateShaftCmdExample
{
    public void CreateComplexShaft()
    {
        try
        {
            // Создание команды
            CreateShaftCmd cmd = new CreateShaftCmd();
            cmd.Document = GetActiveDocument(); // Получение активного документа
            
            // Создание данных вала
            ShaftData shaftData = CreateComplexShaftData();
            
            // Проверка валидности данных
            if (!shaftData.Validate())
            {
                Console.WriteLine("Невалидные данные вала");
                return;
            }
            
            // Установка данных в команду
            cmd.ShaftData = shaftData;
            
            // Создание вала
            Console.WriteLine("Начало создания вала...");
            bool success = cmd.CreateShaft(shaftData);
            
            if (success)
            {
                Console.WriteLine("Вал успешно создан");
                
                // Регенерация модели для обновления отображения
                if (cmd.RegenerateModel())
                {
                    Console.WriteLine("Модель успешно обновлена");
                }
                else
                {
                    Console.WriteLine("Ошибка обновления модели");
                }
            }
            else
            {
                Console.WriteLine("Ошибка создания вала");
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Исключение при создании вала: {ex.Message}");
        }
    }
    
    private static ShaftData CreateComplexShaftData()
    {
        ShaftData data = new ShaftData();
        data.Name = "Сложный вал";
        data.Material = "Сталь 40Х";
        data.Notes = "Вал с множеством ступеней и элементов";
        
        // Основная ступень
        ShaftStep mainStep = new ShaftStep(PrimitiveType.Cylinder, 60.0, 200.0);
        mainStep.Name = "Основная ступень";
        
        // Добавление обработок кромок
        ElementEdge startRadius = new ElementEdge();
        startRadius.SetRadius(3.0, EdgePosition.Start);
        mainStep.AddEdge(startRadius);
        
        ElementEdge endRadius = new ElementEdge();
        endRadius.SetRadius(3.0, EdgePosition.End);
        mainStep.AddEdge(endRadius);
        
        data.AddStep(mainStep);
        
        // Переходная ступень
        ShaftStep transitionStep = new ShaftStep(PrimitiveType.Cone, 60.0, 40.0, 80.0);
        transitionStep.Name = "Переходная ступень";
        data.AddStep(transitionStep);
        
        // Хвостовик
        ShaftStep stubStep = new ShaftStep(PrimitiveType.Cylinder, 30.0, 100.0);
        stubStep.Name = "Хвостовик";
        data.AddStep(stubStep);
        
        // Добавление отверстий
        ShaftHole keyHole = new ShaftHole(HoleType.Radial, 12.0, 100.0);
        keyHole.Name = "Отверстие под шпонку";
        keyHole.AddChamfer(1.0);
        data.AddHole(keyHole);
        
        return data;
    }
    
    public void CreateShaftPreview()
    {
        try
        {
            // Создание команды для предварительного просмотра
            CreateShaftCmd previewCmd = new CreateShaftCmd();
            previewCmd.Document = GetActiveDocument();
            previewCmd.IsPreview = true; // Включить режим предпросмотра
            
            // Создание данных вала
            ShaftData shaftData = CreateSampleShaftData();
            
            // Создание предварительного просмотра
            Console.WriteLine("Создание предварительного просмотра...");
            bool previewSuccess = previewCmd.CreatePreview(shaftData);
            
            if (previewSuccess)
            {
                Console.WriteLine("Предварительный просмотр создан успешно");
            }
            else
            {
                Console.WriteLine("Ошибка создания предварительного просмотра");
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Исключение при создании предварительного просмотра: {ex.Message}");
        }
    }
}