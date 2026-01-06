# Шпаргалка DialogData T-Flex CAD API

## Основная информация

**Класс:** DialogData
**Пространство имен:** TFlex.Shaft.Plugin.Interface
**Тип:** Класс данных
**Назначение:** Представляет данные диалога для управления параметрами вала в системе проектирования T-Flex CAD

## Основные свойства

| Свойство | Тип | Описание | Использование |
|----------|-----|----------|---------------|
| Steps | List<ShaftStep> | Ступени вала | Список ступеней вала для отображения в диалоге |
| Holes | List<ShaftHole> | Отверстия вала | Список отверстий вала для отображения в диалоге |
| SelectedStep | ShaftStep | Выбранная ступень | Текущая выбранная ступень для редактирования |
| SelectedHole | ShaftHole | Выбранное отверстие | Текущее выбранное отверстие для редактирования |
| IsModified | bool | Флаг модификации | Указывает, были ли внесены изменения в данные |
| ValidationErrors | List<string> | Ошибки валидации | Список ошибок валидации данных |
| Name | string | Название вала | Имя вала для идентификации |
| Material | string | Материал вала | Материал, из которого изготовлен вал |
| Notes | string | Примечания | Дополнительная информация о вале |

## Основные методы

### Конструкторы

#### DialogData()
**Описание:** Создает новый экземпляр DialogData
**Параметры:** Нет
**Использование:** Инициализация пустых данных диалога

#### DialogData(ShaftData shaftData)
**Описание:** Создает новый экземпляр DialogData на основе данных вала
**Параметры:** shaftData (ShaftData) - данные вала
**Использование:** Создание данных диалога из существующих данных вала

### Методы управления ступенями

#### AddStep(ShaftStep step)
**Возвращаемый тип:** void
**Описание:** Добавляет ступень в список
**Параметры:** step (ShaftStep) - ступень для добавления
**Использование:** Добавление новой ступени в диалог

#### RemoveStep(ShaftStep step)
**Возвращаемый тип:** bool
**Описание:** Удаляет ступень из списка
**Параметры:** step (ShaftStep) - ступень для удаления
**Использование:** Удаление ступени из диалога

#### MoveStepUp(ShaftStep step)
**Возвращаемый тип:** bool
**Описание:** Перемещает ступень вверх в списке
**Параметры:** step (ShaftStep) - ступень для перемещения
**Использование:** Изменение порядка ступеней

#### MoveStepDown(ShaftStep step)
**Возвращаемый тип:** bool
**Описание:** Перемещает ступень вниз в списке
**Параметры:** step (ShaftStep) - ступень для перемещения
**Использование:** Изменение порядка ступеней

### Методы управления отверстиями

#### AddHole(ShaftHole hole)
**Возвращаемый тип:** void
**Описание:** Добавляет отверстие в список
**Параметры:** hole (ShaftHole) - отверстие для добавления
**Использование:** Добавление нового отверстия в диалог

#### RemoveHole(ShaftHole hole)
**Возвращаемый тип:** bool
**Описание:** Удаляет отверстие из списка
**Параметры:** hole (ShaftHole) - отверстие для удаления
**Использование:** Удаление отверстия из диалога

### Методы управления выбором

#### SelectStep(ShaftStep step)
**Возвращаемый тип:** void
**Описание:** Устанавливает выбранную ступень
**Параметры:** step (ShaftStep) - ступень для выбора
**Использование:** Выбор ступени для редактирования

#### SelectHole(ShaftHole hole)
**Возвращаемый тип:** void
**Описание:** Устанавливает выбранное отверстие
**Параметры:** hole (ShaftHole) - отверстие для выбора
**Использование:** Выбор отверстия для редактирования

#### ClearSelection()
**Возвращаемый тип:** void
**Описание:** Очищает текущий выбор
**Параметры:** Нет
**Использование:** Сброс выбора элементов

### Методы валидации

#### Validate()
**Возвращаемый тип:** bool
**Описание:** Проверяет валидность всех данных
**Параметры:** Нет
**Использование:** Проверка корректности всех данных диалога

#### GetValidationErrors()
**Возвращаемый тип:** List<string>
**Описание:** Возвращает список ошибок валидации
**Параметры:** Нет
**Использование:** Получение детализированных ошибок валидации

### Методы управления состоянием

#### MarkAsModified()
**Возвращаемый тип:** void
**Описание:** Помечает данные как модифицированные
**Параметры:** Нет
**Использование:** Установка флага модификации

#### MarkAsUnmodified()
**Возвращаемый тип:** void
**Описание:** Помечает данные как немодифицированные
**Параметры:** Нет
**Использование:** Сброс флага модификации

#### Reset()
**Возвращаемый тип:** void
**Описание:** Сбрасывает данные к исходному состоянию
**Параметры:** Нет
**Использование:** Восстановление исходных данных

### Методы сериализации

#### ToShaftData()
**Возвращаемый тип:** ShaftData
**Описание:** Преобразует данные диалога в данные вала
**Параметры:** Нет
**Использование:** Получение данных вала для создания геометрии

## Примеры использования

### Создание и инициализация данных диалога

```csharp
// Создание пустых данных диалога
DialogData dialogData = new DialogData();
dialogData.Name = "Новый вал";
dialogData.Material = "Сталь 45";
dialogData.Notes = "Вал для редуктора";

// Создание данных диалога из существующих данных вала
ShaftData shaftData = GetShaftData(); // Получение данных вала
DialogData dialogDataFromShaft = new DialogData(shaftData);
dialogDataFromShaft.Name = shaftData.Name;
dialogDataFromShaft.Material = shaftData.Material;
```

### Работа со ступенями

```csharp
// Создание данных диалога
DialogData dialogData = new DialogData();

// Добавление ступеней
ShaftStep step1 = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
step1.Name = "Основная ступень";

ShaftStep step2 = new ShaftStep(PrimitiveType.Cone, 50.0, 30.0, 50.0);
step2.Name = "Конический переход";

ShaftStep step3 = new ShaftStep(PrimitiveType.Cylinder, 30.0, 80.0);
step3.Name = "Хвостовик";

dialogData.AddStep(step1);
dialogData.AddStep(step2);
dialogData.AddStep(step3);

// Выбор ступени для редактирования
dialogData.SelectStep(step1);

// Перемещение ступени вверх/вниз
dialogData.MoveStepDown(step1); // Переместить step1 вниз
dialogData.MoveStepUp(step3); // Переместить step3 вверх

// Удаление ступени
dialogData.RemoveStep(step2);
```

### Работа с отверстиями

```csharp
// Создание данных диалога
DialogData dialogData = new DialogData();

// Добавление отверстий
ShaftHole hole1 = new ShaftHole(HoleType.Radial, 10.0, 50.0);
hole1.Name = "Радиальное отверстие";

ShaftHole hole2 = new ShaftHole();
hole2.SetEnd(12.0, 150.0, 25.0);
hole2.Name = "Торцевое отверстие";

dialogData.AddHole(hole1);
dialogData.AddHole(hole2);

// Выбор отверстия для редактирования
dialogData.SelectHole(hole1);

// Удаление отверстия
dialogData.RemoveHole(hole2);
```

### Валидация данных

```csharp
// Создание данных диалога
DialogData dialogData = new DialogData();
dialogData.Name = "Тестовый вал";

// Добавление ступеней и отверстий
ShaftStep step = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
dialogData.AddStep(step);

ShaftHole hole = new ShaftHole(HoleType.Radial, 10.0, 50.0);
dialogData.AddHole(hole);

// Проверка валидности
if (dialogData.Validate())
{
    Console.WriteLine("Данные диалога валидны");
}
else
{
    Console.WriteLine("Данные диалога не валидны");
    
    // Получение ошибок валидации
    List<string> errors = dialogData.GetValidationErrors();
    foreach (string error in errors)
    {
        Console.WriteLine($"Ошибка: {error}");
    }
}
```

### Управление состоянием модификации

```csharp
// Создание данных диалога
DialogData dialogData = new DialogData();

// Проверка состояния модификации
Console.WriteLine($"Модифицирован: {dialogData.IsModified}"); // False

// Добавление ступени
ShaftStep step = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
dialogData.AddStep(step);

// Проверка состояния модификации
Console.WriteLine($"Модифицирован: {dialogData.IsModified}"); // True

// Пометка как немодифицированный
dialogData.MarkAsUnmodified();
Console.WriteLine($"Модифицирован: {dialogData.IsModified}"); // False

// Сброс данных
dialogData.Reset();
Console.WriteLine($"Ступеней: {dialogData.Steps.Count}"); // 0
```

## Практические рекомендации

### Рекомендации по использованию

1. **Используйте конструкторы для быстрого создания данных диалога**
   - Используйте конструктор с ShaftData для создания данных из существующего вала
   - Это упрощает код и повышает читаемость

2. **Проверяйте валидность данных перед использованием**
   - Всегда проверяйте валидность данных перед применением изменений
   - Это помогает избежать ошибок в дальнейшей обработке

3. **Используйте методы управления выбором для работы с элементами**
   - Используйте SelectStep/SelectHole для выбора элементов для редактирования
   - Используйте ClearSelection для сброса выбора

4. **Управляйте состоянием модификации корректно**
   - Используйте MarkAsModified/MarkAsUnmodified для управления флагом модификации
   - Используйте Reset для восстановления исходных данных

### Антипаттерны

1. **Не игнорируйте проверку валидности**
   - Всегда проверяйте валидность данных перед применением изменений
   - Не используйте некорректные данные для создания геометрии

2. **Не забывайте управлять состоянием модификации**
   - Всегда помечайте данные как модифицированные при внесении изменений
   - Сбрасывайте флаг модификации после сохранения изменений

3. **Не добавляйте дублирующие элементы**
   - Проверяйте наличие элементов перед добавлением
   - Используйте уникальные идентификаторы для элементов

## Распространенные ошибки

### Ошибка 1: Отсутствие проверки валидности перед применением изменений

```csharp
// Неправильно
DialogData dialogData = new DialogData();
// Добавление некорректных данных
ShaftStep invalidStep = new ShaftStep(PrimitiveType.Cylinder, -10.0, 100.0); // Отрицательный диаметр
dialogData.AddStep(invalidStep);

// Применение изменений без проверки валидности
ShaftData shaftData = dialogData.ToShaftData(); // Ошибка: некорректные данные

// Правильно
DialogData dialogData = new DialogData();
ShaftStep invalidStep = new ShaftStep(PrimitiveType.Cylinder, -10.0, 100.0);
dialogData.AddStep(invalidStep);

// Проверка валидности перед применением
if (dialogData.Validate())
{
    ShaftData shaftData = dialogData.ToShaftData();
}
else
{
    Console.WriteLine("Данные не валидны, невозможно создать вал");
}
```

### Ошибка 2: Неправильное управление состоянием модификации

```csharp
// Неправильно
DialogData dialogData = new DialogData();
ShaftStep step = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
dialogData.AddStep(step);

// Забыли пометить как модифицированный
if (dialogData.IsModified)
{
    // Этот код не выполнится, так как флаг не установлен
    SaveChanges(dialogData);
}

// Правильно
DialogData dialogData = new DialogData();
ShaftStep step = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
dialogData.AddStep(step);
dialogData.MarkAsModified(); // Правильно: помечаем как модифицированный

if (dialogData.IsModified)
{
    SaveChanges(dialogData); // Этот код выполнится
}
```

## Лучшие практики

### 1. Использование фабричного метода для создания данных диалога

```csharp
public static class DialogDataFactory
{
    public static DialogData CreateFromShaftData(ShaftData shaftData)
    {
        DialogData dialogData = new DialogData(shaftData);
        dialogData.Name = shaftData.Name;
        dialogData.Material = shaftData.Material;
        dialogData.Notes = shaftData.Notes;
        return dialogData;
    }
    
    public static DialogData CreateNew(string name, string material = "Сталь 45")
    {
        DialogData dialogData = new DialogData();
        dialogData.Name = name;
        dialogData.Material = material;
        dialogData.Notes = "";
        return dialogData;
    }
    
    public static DialogData CreateTemplate(string templateName)
    {
        DialogData dialogData = new DialogData();
        dialogData.Name = $"Новый {templateName}";
        
        switch (templateName.ToLower())
        {
            case "ступенчатый вал":
                CreateSteppedShaftTemplate(dialogData);
                break;
            case "гладкий вал":
                CreateSmoothShaftTemplate(dialogData);
                break;
            case "хвостовик":
                CreateStubShaftTemplate(dialogData);
                break;
        }
        
        return dialogData;
    }
    
    private static void CreateSteppedShaftTemplate(DialogData dialogData)
    {
        // Создание шаблона ступенчатого вала
        ShaftStep step1 = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
        step1.Name = "Основная ступень";
        dialogData.AddStep(step1);
        
        ShaftStep step2 = new ShaftStep(PrimitiveType.Cylinder, 30.0, 80.0);
        step2.Name = "Хвостовик";
        dialogData.AddStep(step2);
        
        dialogData.Material = "Сталь 45";
    }
    
    private static void CreateSmoothShaftTemplate(DialogData dialogData)
    {
        // Создание шаблона гладкого вала
        ShaftStep step = new ShaftStep(PrimitiveType.Cylinder, 40.0, 200.0);
        step.Name = "Гладкий вал";
        dialogData.AddStep(step);
        
        dialogData.Material = "Сталь 45";
    }
    
    private static void CreateStubShaftTemplate(DialogData dialogData)
    {
        // Создание шаблона хвостовика
        ShaftStep step = new ShaftStep(PrimitiveType.Cylinder, 30.0, 150.0);
        step.Name = "Хвостовик";
        dialogData.AddStep(step);
        
        dialogData.Material = "Сталь 45";
    }
}

// Использование
DialogData fromShaft = DialogDataFactory.CreateFromShaftData(shaftData);
DialogData newDialog = DialogDataFactory.CreateNew("Новый вал", "Сталь 20");
DialogData templateDialog = DialogDataFactory.CreateTemplate("ступенчатый вал");
```

### 2. Проверка совместимости данных

```csharp
public static class DialogDataValidator
{
    public static bool IsCompatible(DialogData dialogData)
    {
        // Проверка базовых параметров
        if (string.IsNullOrEmpty(dialogData.Name))
            return false;
            
        if (string.IsNullOrEmpty(dialogData.Material))
            return false;
            
        // Проверка ступеней
        foreach (ShaftStep step in dialogData.Steps)
        {
            if (!step.Validate())
                return false;
        }
        
        // Проверка отверстий
        foreach (ShaftHole hole in dialogData.Holes)
        {
            if (!hole.Validate())
                return false;
        }
        
        return true;
    }
    
    public static List<string> GetCompatibilityErrors(DialogData dialogData)
    {
        List<string> errors = new List<string>();
        
        if (string.IsNullOrEmpty(dialogData.Name))
            errors.Add("Не указано имя вала");
            
        if (string.IsNullOrEmpty(dialogData.Material))
            errors.Add("Не указан материал вала");
            
        // Проверка ступеней
        for (int i = 0; i < dialogData.Steps.Count; i++)
        {
            if (!dialogData.Steps[i].Validate())
            {
                errors.Add($"Ступень {i + 1} содержит ошибки");
            }
        }
        
        // Проверка отверстий
        for (int i = 0; i < dialogData.Holes.Count; i++)
        {
            if (!dialogData.Holes[i].Validate())
            {
                errors.Add($"Отверстие {i + 1} содержит ошибки");
            }
        }
        
        return errors;
    }
}

// Использование
DialogData dialogData = GetDialogData();
if (DialogDataValidator.IsCompatible(dialogData))
{
    Console.WriteLine("Данные диалога совместимы");
}
else
{
    List<string> errors = DialogDataValidator.GetCompatibilityErrors(dialogData);
    foreach (string error in errors)
    {
        Console.WriteLine($"Ошибка: {error}");
    }
}
```

### 3. Создание шаблонов данных диалога

```csharp
public static class DialogDataTemplates
{
    // Создание шаблона для редукторного вала
    public static DialogData CreateReducerShaftTemplate()
    {
        DialogData dialogData = new DialogData();
        dialogData.Name = "Редукторный вал";
        dialogData.Material = "Сталь 40Х";
        dialogData.Notes = "Вал для цилиндрического редуктора";
        
        // Основная ступень
        ShaftStep mainStep = new ShaftStep(PrimitiveType.Cylinder, 50.0, 150.0);
        mainStep.Name = "Основная ступень";
        
        // Добавление обработок кромок
        ElementEdge startRadius = new ElementEdge();
        startRadius.SetRadius(2.0, EdgePosition.Start);
        mainStep.AddEdge(startRadius);
        
        ElementEdge endRadius = new ElementEdge();
        endRadius.SetRadius(2.0, EdgePosition.End);
        mainStep.AddEdge(endRadius);
        
        dialogData.AddStep(mainStep);
        
        // Хвостовик
        ShaftStep stubStep = new ShaftStep(PrimitiveType.Cylinder, 30.0, 100.0);
        stubStep.Name = "Хвостовик";
        dialogData.AddStep(stubStep);
        
        // Добавление отверстий
        ShaftHole keyHole = new ShaftHole(HoleType.Radial, 10.0, 75.0);
        keyHole.Name = "Отверстие под шпонку";
        dialogData.AddHole(keyHole);
        
        return dialogData;
    }
    
    // Создание шаблона для промежуточного вала
    public static DialogData CreateIntermediateShaftTemplate()
    {
        DialogData dialogData = new DialogData();
        dialogData.Name = "Промежуточный вал";
        dialogData.Material = "Сталь 45";
        dialogData.Notes = "Промежуточный вал редуктора";
        
        // Первая ступень
        ShaftStep step1 = new ShaftStep(PrimitiveType.Cylinder, 40.0, 80.0);
        step1.Name = "Первая ступень";
        dialogData.AddStep(step1);
        
        // Переходная ступень
        ShaftStep step2 = new ShaftStep(PrimitiveType.Cone, 40.0, 50.0, 50.0);
        step2.Name = "Переходная ступень";
        dialogData.AddStep(step2);
        
        // Вторая ступень
        ShaftStep step3 = new ShaftStep(PrimitiveType.Cylinder, 50.0, 100.0);
        step3.Name = "Вторая ступень";
        dialogData.AddStep(step3);
        
        // Хвостовик
        ShaftStep step4 = new ShaftStep(PrimitiveType.Cylinder, 35.0, 70.0);
        step4.Name = "Хвостовик";
        dialogData.AddStep(step4);
        
        return dialogData;
    }
}

// Использование
DialogData reducerShaft = DialogDataTemplates.CreateReducerShaftTemplate();
DialogData intermediateShaft = DialogDataTemplates.CreateIntermediateShaftTemplate();
```

## Интеграция с другими компонентами

### ShaftData

DialogData использует ShaftData для инициализации и преобразования данных.

### GeneralDialog

DialogData используется в GeneralDialog для отображения и редактирования параметров вала.

### CreateShaftCmd

DialogData используется в CreateShaftCmd для получения параметров вала перед созданием геометрии.

### ShaftStep

DialogData использует ShaftStep для хранения информации о ступенях вала.

### ShaftHole

DialogData использует ShaftHole для хранения информации об отверстиях вала.

## Сериализация

### XML сериализация

```csharp
// Пример XML представления
/*
<DialogData>
    <Name>Тестовый вал</Name>
    <Material>Сталь 45</Material>
    <Notes>Вал для тестирования</Notes>
    <IsModified>true</IsModified>
    <Steps>
        <ShaftStep>
            <Type>Cylinder</Type>
            <Diameter>50.0</Diameter>
            <Length>100.0</Length>
            <Name>Основная ступень</Name>
        </ShaftStep>
    </Steps>
    <Holes>
        <ShaftHole>
            <Type>Radial</Type>
            <Diameter>10.0</Diameter>
            <Position>50.0</Position>
            <Name>Радиальное отверстие</Name>
        </ShaftHole>
    </Holes>
</DialogData>
*/
```

## Тестирование

### Основные сценарии тестирования

1. **Проверка создания данных диалога**
   - Создание пустых данных диалога
   - Создание данных диалога из ShaftData

2. **Проверка работы со ступенями**
   - Добавление ступеней
   - Удаление ступеней
   - Перемещение ступеней
   - Выбор ступеней

3. **Проверка работы с отверстиями**
   - Добавление отверстий
   - Удаление отверстий
   - Выбор отверстий

4. **Проверка валидации данных**
   - Валидация корректных данных
   - Валидация некорректных данных
   - Получение ошибок валидации

5. **Проверка управления состоянием**
   - Управление флагом модификации
   - Сброс данных
   - Преобразование в ShaftData

## Производительность

### Рекомендации по оптимизации

1. **Используйте кэширование для часто создаваемых данных диалога**
   - Создавайте шаблоны для часто используемых конфигураций
   - Используйте клонирование вместо повторного создания

2. **Минимизируйте количество проверок валидности**
   - Проверяйте валидность только при необходимости
   - Кэшируйте результаты проверок

3. **Используйте пакетную обработку для множества элементов**
   - Обрабатывайте элементы пакетами
   - Минимизируйте количество операций с коллекциями

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
- GeneralDialog - класс основного диалога
- CreateShaftCmd - команда создания вала
- ShaftStep - класс ступени вала
- ShaftHole - класс отверстия в валу

### Примеры в коде

```csharp
// Полный пример использования DialogData
public class DialogDataExample
{
    public void CreateComplexDialogData()
    {
        // Создание данных диалога
        DialogData dialogData = new DialogData();
        dialogData.Name = "Сложный вал";
        dialogData.Material = "Сталь 40Х";
        dialogData.Notes = "Вал с множеством ступеней и отверстий";
        
        // Добавление ступеней
        ShaftStep mainStep = new ShaftStep(PrimitiveType.Cylinder, 60.0, 200.0);
        mainStep.Name = "Основная ступень";
        
        // Добавление обработок кромок
        ElementEdge startRadius = new ElementEdge();
        startRadius.SetRadius(3.0, EdgePosition.Start);
        mainStep.AddEdge(startRadius);
        
        ElementEdge endRadius = new ElementEdge();
        endRadius.SetRadius(3.0, EdgePosition.End);
        mainStep.AddEdge(endRadius);
        
        dialogData.AddStep(mainStep);
        
        ShaftStep transitionStep = new ShaftStep(PrimitiveType.Cone, 60.0, 40.0, 80.0);
        transitionStep.Name = "Переходная ступень";
        dialogData.AddStep(transitionStep);
        
        ShaftStep stubStep = new ShaftStep(PrimitiveType.Cylinder, 30.0, 100.0);
        stubStep.Name = "Хвостовик";
        dialogData.AddStep(stubStep);
        
        // Добавление отверстий
        ShaftHole keyHole = new ShaftHole(HoleType.Radial, 12.0, 100.0);
        keyHole.Name = "Отверстие под шпонку";
        keyHole.AddChamfer(1.0);
        dialogData.AddHole(keyHole);
        
        ShaftHole endHole = new ShaftHole();
        endHole.SetEnd(15.0, 350.0, 30.0);
        endHole.Name = "Торцевое отверстие";
        dialogData.AddHole(endHole);
        
        // Проверка валидности
        if (dialogData.Validate())
        {
            Console.WriteLine($"Данные диалога '{dialogData.Name}' созданы успешно");
            Console.WriteLine($"Ступеней: {dialogData.Steps.Count}");
            Console.WriteLine($"Отверстий: {dialogData.Holes.Count}");
            Console.WriteLine($"Материал: {dialogData.Material}");
            Console.WriteLine($"Модифицирован: {dialogData.IsModified}");
        }
        else
        {
            Console.WriteLine("Ошибка создания данных диалога");
            
            // Получение ошибок валидации
            List<string> errors = dialogData.GetValidationErrors();
            foreach (string error in errors)
            {
                Console.WriteLine($"Ошибка: {error}");
            }
        }
    }
    
    public void ProcessDialogData(DialogData dialogData)
    {
        // Выбор ступени для редактирования
        if (dialogData.Steps.Count > 0)
        {
            dialogData.SelectStep(dialogData.Steps[0]);
            Console.WriteLine($"Выбрана ступень: {dialogData.SelectedStep?.Name}");
        }
        
        // Выбор отверстия для редактирования
        if (dialogData.Holes.Count > 0)
        {
            dialogData.SelectHole(dialogData.Holes[0]);
            Console.WriteLine($"Выбрано отверстие: {dialogData.SelectedHole?.Name}");
        }
        
        // Преобразование в данные вала
        ShaftData shaftData = dialogData.ToShaftData();
        Console.WriteLine($"Созданы данные вала: {shaftData.Name}");
    }
}