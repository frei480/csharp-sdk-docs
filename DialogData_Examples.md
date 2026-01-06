# DialogData в T-Flex CAD API

## Описание
DialogData - это класс, представляющий данные диалогового окна в T-Flex CAD API. Он используется для хранения и управления данными, отображаемыми в пользовательском интерфейсе плагина.

## Основные свойства
- ShaftSteps - Список ступеней вала
- ShaftHoles - Список отверстий в валу
- SelectedStepIndex - Индекс выбранной ступени
- SelectedHoleIndex - Индекс выбранного отверстия
- SelectedElementIndex - Индекс выбранного элемента
- IsModified - Флаг модификации данных

## Примеры использования

### 1. Создание и инициализация DialogData

```csharp
// Создание нового экземпляра DialogData
DialogData CreateNewDialogData()
{
    DialogData data = new DialogData();
    
    // Инициализация списков
    data.ShaftSteps = new List<ShaftStep>();
    data.ShaftHoles = new List<ShaftHole>();
    
    // Установка начальных значений
    data.SelectedStepIndex = -1;
    data.SelectedHoleIndex = -1;
    data.SelectedElementIndex = -1;
    data.IsModified = false;
    
    return data;
}

// Создание DialogData с начальными ступенями
DialogData CreateDialogDataWithSteps(List<ShaftStep> initialSteps)
{
    DialogData data = new DialogData();
    data.ShaftSteps = new List<ShaftStep>(initialSteps);
    data.ShaftHoles = new List<ShaftHole>();
    data.SelectedStepIndex = -1;
    data.SelectedHoleIndex = -1;
    data.SelectedElementIndex = -1;
    data.IsModified = false;
    
    return data;
}
```

### 2. Работа с данными ступеней

```csharp
// Добавление новой ступени
public void AddStep(DialogData data, ShaftStep step)
{
    data.ShaftSteps.Add(step);
    data.IsModified = true;
}

// Удаление ступени
public void RemoveStep(DialogData data, int stepIndex)
{
    if (stepIndex >= 0 && stepIndex < data.ShaftSteps.Count)
    {
        // Удалить связанные отверстия
        data.ShaftHoles.RemoveAll(h => h.StepIndex == stepIndex);
        
        // Обновить индексы отверстий
        foreach (var hole in data.ShaftHoles.Where(h => h.StepIndex > stepIndex))
        {
            hole.StepIndex--;
        }
        
        // Удалить ступень
        data.ShaftSteps.RemoveAt(stepIndex);
        data.IsModified = true;
        
        // Сбросить выбор, если он указывал на удаленную ступень
        if (data.SelectedStepIndex == stepIndex)
        {
            data.SelectedStepIndex = -1;
        }
        else if (data.SelectedStepIndex > stepIndex)
        {
            data.SelectedStepIndex--;
        }
    }
}

// Получение ступени по индексу
public ShaftStep GetStep(DialogData data, int index)
{
    if (index >= 0 && index < data.ShaftSteps.Count)
    {
        return data.ShaftSteps[index];
    }
    return null;
}

// Обновление ступени
public void UpdateStep(DialogData data, int index, ShaftStep updatedStep)
{
    if (index >= 0 && index < data.ShaftSteps.Count)
    {
        data.ShaftSteps[index] = updatedStep;
        data.IsModified = true;
    }
}
```

### 3. Работа с данными отверстий

```csharp
// Добавление нового отверстия
public void AddHole(DialogData data, ShaftHole hole)
{
    data.ShaftHoles.Add(hole);
    data.IsModified = true;
}

// Удаление отверстия
public void RemoveHole(DialogData data, int holeIndex)
{
    if (holeIndex >= 0 && holeIndex < data.ShaftHoles.Count)
    {
        data.ShaftHoles.RemoveAt(holeIndex);
        data.IsModified = true;
        
        // Сбросить выбор, если он указывал на удаленное отверстие
        if (data.SelectedHoleIndex == holeIndex)
        {
            data.SelectedHoleIndex = -1;
        }
        else if (data.SelectedHoleIndex > holeIndex)
        {
            data.SelectedHoleIndex--;
        }
    }
}

// Получение отверстия по индексу
public ShaftHole GetHole(DialogData data, int index)
{
    if (index >= 0 && index < data.ShaftHoles.Count)
    {
        return data.ShaftHoles[index];
    }
    return null;
}

// Получение отверстий для определенной ступени
public List<ShaftHole> GetHolesForStep(DialogData data, int stepIndex)
{
    return data.ShaftHoles.Where(h => h.StepIndex == stepIndex).ToList();
}
```

### 4. Управление выбором

```csharp
// Установка выбранной ступени
public void SetSelectedStep(DialogData data, int stepIndex)
{
    if (stepIndex >= -1 && stepIndex < data.ShaftSteps.Count)
    {
        data.SelectedStepIndex = stepIndex;
        // Сбросить выбор отверстия и элемента при смене ступени
        data.SelectedHoleIndex = -1;
        data.SelectedElementIndex = -1;
    }
}

// Установка выбранного отверстия
public void SetSelectedHole(DialogData data, int holeIndex)
{
    if (holeIndex >= -1 && holeIndex < data.ShaftHoles.Count)
    {
        data.SelectedHoleIndex = holeIndex;
        // Сбросить выбор элемента при смене отверстия
        data.SelectedElementIndex = -1;
    }
}

// Установка выбранного элемента
public void SetSelectedElement(DialogData data, int elementIndex)
{
    data.SelectedElementIndex = elementIndex;
}

// Проверка наличия выбора
public bool HasSelection(DialogData data)
{
    return data.SelectedStepIndex >= 0 || data.SelectedHoleIndex >= 0 || data.SelectedElementIndex >= 0;
}

// Сброс всех выборов
public void ClearSelections(DialogData data)
{
    data.SelectedStepIndex = -1;
    data.SelectedHoleIndex = -1;
    data.SelectedElementIndex = -1;
}
```

### 5. Работа с состоянием данных

```csharp
// Проверка наличия изменений
public bool IsDataModified(DialogData data)
{
    return data.IsModified;
}

// Сброс флага модификации
public void ResetModificationFlag(DialogData data)
{
    data.IsModified = false;
}

// Получение общего количества ступеней
public int GetStepCount(DialogData data)
{
    return data.ShaftSteps.Count;
}

// Получение общего количества отверстий
public int GetHoleCount(DialogData data)
{
    return data.ShaftHoles.Count;
}

// Получение максимального диаметра вала
public double GetMaxDiameter(DialogData data)
{
    if (data.ShaftSteps.Count == 0)
        return 0;
        
    return data.ShaftSteps.Max(s => GetMaxDiameter(s));
}

// Вспомогательный метод для получения максимального диаметра ступени
private double GetMaxDiameter(ShaftStep step)
{
    switch (step.PrimitiveType)
    {
        case PrimitiveType.Cylinder:
            return step.PrimitiveCylinder.D.Value;
        case PrimitiveType.Cone:
            return Math.Max(step.PrimitiveCone.D.Value, step.PrimitiveCone.D2.Value);
        case PrimitiveType.Prisma:
            return step.PrimitivePrisma.D.Value;
        default:
            return 0;
    }
}
```

## Практические рекомендации

1. Всегда инициализируйте списки ShaftSteps и ShaftHoles при создании DialogData
2. Используйте флаг IsModified для отслеживания изменений в данных
3. При удалении ступеней не забывайте обновлять индексы связанных отверстий
4. При смене выбора ступени сбрасывайте выбор отверстия и элемента
5. При смене выбора отверстия сбрасывайте выбор элемента
6. Используйте вспомогательные методы для получения данных по индексам с проверкой границ
7. При работе с коллекциями используйте LINQ для фильтрации и поиска
8. Не забывайте сбрасывать флаг IsModified после сохранения данных