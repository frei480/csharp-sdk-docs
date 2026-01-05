# Продвинутые примеры использования класса TFlex.Model.Model2D.Table

## 1. Создание таблицы с пользовательскими стилями

### 1.1. Создание таблицы с различными стилями ячеек

```csharp
public static void CreateTableWithCustomStyles()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание таблицы с пользовательскими стилями");
    
    MultilineText mt = new MultilineText(document);
    mt.BeginEdit();
    mt.X = 100;
    mt.Y = 200;
    
    // Создание настроек таблицы (5 столбцов, 4 строки)
    Table.CreationSettings sett = new Table.CreationSettings(5, 4);
    Table table = mt.CreateTable(sett);
    
    // Создание различных стилей
    Table.CellProperties headerStyle = new Table.CellProperties();
    headerStyle.CellTextVAlign = Table.TextVAlign.Center;
    headerStyle.CellTextHAlign = Table.TextHAlign.Center;
    headerStyle.BackgroundColor = 12632256; // Серый цвет фона
    headerStyle.TextDirection = Table.TextDirection.Normal;
    headerStyle.CellWidth = 30;
    headerStyle.RowHeight = 15;
    
    Table.CellProperties dataStyle = new Table.CellProperties();
    dataStyle.CellTextVAlign = Table.TextVAlign.Top;
    dataStyle.CellTextHAlign = Table.TextHAlign.Left;
    dataStyle.TextDirection = Table.TextDirection.Normal;
    dataStyle.CellWidth = 30;
    dataStyle.RowHeight = 12;
    
    // Применение стилей к ячейкам
    // Заголовки
    for (int i = 0; i < 5; i++)
    {
        table.SetCellProperties(i, headerStyle);
        table.InsertText(i, 0, "Заголовок " + (i + 1));
    }
    
    // Данные
    for (int row = 1; row < 4; row++)
    {
        for (int col = 0; col < 5; col++)
        {
            int cellIndex = row * 5 + col;
            table.SetCellProperties(cellIndex, dataStyle);
            table.InsertText(cellIndex, 0, "Данные " + row + "," + col);
        }
    }
    
    mt.EndEdit();
    document.EndChanges();
}
```

### 1.2. Создание таблицы с различными форматами текста

```csharp
public static void CreateTableWithTextFormats()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание таблицы с форматами текста");
    
    MultilineText mt = new MultilineText(document);
    mt.BeginEdit();
    mt.X = 100;
    mt.Y = 200;
    
    Table.CreationSettings sett = new Table.CreationSettings(3, 3);
    Table table = mt.CreateTable(sett);
    
    // Создание различных форматов текста
    CharFormat boldFormat = new CharFormat();
    boldFormat.isBold = true;
    boldFormat.FontSize = 14;
    
    CharFormat italicFormat = new CharFormat();
    italicFormat.isItalic = true;
    italicFormat.FontSize = 12;
    
    CharFormat underlineFormat = new CharFormat();
    underlineFormat.isUnderline = true;
    underlineFormat.FontSize = 12;
    
    // Заполнение таблицы с различными форматами
    table.InsertText(0, 0, "Жирный текст", boldFormat);
    table.InsertText(1, 0, "Курсив", italicFormat);
    table.InsertText(2, 0, "Подчеркнутый", underlineFormat);
    
    mt.EndEdit();
    document.EndChanges();
}
```

## 2. Работа с объединенными ячейками

### 2.1. Создание таблицы с комплексными объединениями

```csharp
public static void CreateTableWithComplexMerges()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание таблицы с объединениями");
    
    MultilineText mt = new MultilineText(document);
    mt.BeginEdit();
    mt.X = 100;
    mt.Y = 200;
    
    Table.CreationSettings sett = new Table.CreationSettings(4, 4);
    Table table = mt.CreateTable(sett);
    
    // Установка ширины столбцов
    for (int i = 0; i < 16; i++)
    {
        table.SetCellWidth(i, 25);
    }
    
    // Создание заголовка, объединяющего все столбцы
    table.MergeCells(0, 3);
    table.InsertText(0, 0, "Основной заголовок таблицы");
    
    // Создание бокового заголовка, объединяющего строки
    table.MergeCells(4, 12);
    table.InsertText(4, 0, "Боковой заголовок");
    
    // Создание объединенной ячейки в центре
    table.MergeCells(6, 7);
    table.MergeCells(10, 11);
    table.MergeCells(6, 10);
    table.InsertText(6, 0, "Центральная ячейка");
    
    mt.EndEdit();
    document.EndChanges();
}
```

### 2.2. Динамическое объединение ячеек

```csharp
public static void DynamicCellMerging(Table table, int startCell, int endCell)
{
    Document document = table.Document;
    document.BeginChanges("Динамическое объединение");
    
    // Проверка корректности диапазона
    if (startCell >= 0 && endCell < table.CellsCount && startCell < endCell)
    {
        table.MergeCells(startCell, endCell);
        table.InsertText(startCell, 0, "Объединенная ячейка " + startCell + "-" + endCell);
    }
    
    document.EndChanges();
}
```

## 3. Работа с размерами таблицы

### 3.1. Создание таблицы с автоматическим размером

```csharp
public static void CreateTableWithAutoSize()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание таблицы с авто-размером");
    
    MultilineText mt = new MultilineText(document);
    mt.BeginEdit();
    mt.X = 100;
    mt.Y = 200;
    
    Table.CreationSettings sett = new Table.CreationSettings(3, 3);
    Table table = mt.CreateTable(sett);
    
    // Установка свойств с автоматическим размером
    Table.CellProperties prop = new Table.CellProperties();
    prop.RowHeightMode = SizeMode.Auto;
    prop.CellWidthMode = SizeMode.Auto;
    prop.RowWrap = true;
    
    // Применение свойств ко всей таблице
    table.Properties = prop;
    
    // Заполнение таблицы текстом различной длины
    table.InsertText(0, 0, "Короткий");
    table.InsertText(1, 0, "Средний текст");
    table.InsertText(2, 0, "Очень длинный текст, который должен автоматически переноситься на несколько строк");
    
    mt.EndEdit();
    document.EndChanges();
}
```

### 3.2. Динамическое изменение размеров таблицы

```csharp
public static void ResizeTableDynamically(Table table, double newWidth, double newHeight)
{
    Document document = table.Document;
    document.BeginChanges("Динамическое изменение размера");
    
    // Изменение размеров таблицы
    for (int i = 0; i < table.CellsCount; i++)
    {
        table.SetCellWidth(i, newWidth / table.ColumnsCount);
        table.SetCellHeight(i, newHeight / table.RowsCount, SizeMode.Exact);
    }
    
    document.EndChanges();
}
```

## 4. Работа с событиями таблицы

### 4.1. Отслеживание изменений в таблице

```csharp
public static void CreateTableWithEventHandling()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание таблицы с обработкой событий");
    
    MultilineText mt = new MultilineText(document);
    mt.BeginEdit();
    mt.X = 100;
    mt.Y = 200;
    
    Table.CreationSettings sett = new Table.CreationSettings(2, 2);
    Table table = mt.CreateTable(sett);
    
    // Добавление обработчиков событий (если доступны в API)
    // table.CellTextChanged += OnCellTextChanged;
    // table.TableResized += OnTableResized;
    
    mt.EndEdit();
    document.EndChanges();
}

// Обработчик изменения текста в ячейке
private static void OnCellTextChanged(object sender, EventArgs e)
{
    // Обработка изменения текста
    Console.WriteLine("Текст в ячейке изменен");
}

// Обработчик изменения размера таблицы
private static void OnTableResized(object sender, EventArgs e)
{
    // Обработка изменения размера
    Console.WriteLine("Размер таблицы изменен");
}
```

## 5. Интеграция таблицы с другими объектами

### 5.1. Создание таблицы как части сложного объекта

```csharp
public static void CreateTableAsPartOfComplexObject()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание сложного объекта с таблицей");
    
    // Создание основного объекта
    MultilineText mainObject = new MultilineText(document);
    mainObject.BeginEdit();
    mainObject.X = 50;
    mainObject.Y = 50;
    mainObject.InsertText("Основной объект");
    
    // Создание таблицы как части объекта
    MultilineText tableContainer = new MultilineText(document);
    tableContainer.BeginEdit();
    tableContainer.X = 50;
    tableContainer.Y = 100;
    
    Table.CreationSettings sett = new Table.CreationSettings(3, 2);
    Table table = tableContainer.CreateTable(sett);
    
    // Заполнение таблицы
    table.InsertText(0, 0, "Параметр 1");
    table.InsertText(1, 0, "Параметр 2");
    table.InsertText(2, 0, "Параметр 3");
    table.InsertText(3, 0, "Значение 1");
    table.InsertText(4, 0, "Значение 2");
    table.InsertText(5, 0, "Значение 3");
    
    tableContainer.EndEdit();
    mainObject.EndEdit();
    
    document.EndChanges();
}
```

### 5.2. Создание таблицы с гиперссылками

```csharp
public static void CreateTableWithHyperlinks()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание таблицы с гиперссылками");
    
    MultilineText mt = new MultilineText(document);
    mt.BeginEdit();
    mt.X = 100;
    mt.Y = 200;
    
    Table.CreationSettings sett = new Table.CreationSettings(2, 2);
    Table table = mt.CreateTable(sett);
    
    // Создание текста с гиперссылкой (если поддерживается API)
    // CharFormat linkFormat = new CharFormat();
    // linkFormat.Color = 16711680; // Синий цвет
    // linkFormat.isUnderline = true;
    // table.InsertText(0, 0, "Ссылка на документ", linkFormat);
    
    mt.EndEdit();
    document.EndChanges();
}
```

## 6. Оптимизация производительности

### 6.1. Эффективное создание больших таблиц

```csharp
public static void CreateLargeTableEfficiently(int rows, int columns)
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание большой таблицы");
    
    MultilineText mt = new MultilineText(document);
    mt.BeginEdit();
    mt.X = 100;
    mt.Y = 200;
    
    Table.CreationSettings sett = new Table.CreationSettings(columns, rows);
    Table table = mt.CreateTable(sett);
    
    // Предварительная настройка свойств
    Table.CellProperties defaultProp = new Table.CellProperties();
    defaultProp.CellWidth = 20;
    defaultProp.RowHeight = 15;
    defaultProp.CellTextVAlign = Table.TextVAlign.Center;
    defaultProp.CellTextHAlign = Table.TextHAlign.Center;
    
    // Быстрое заполнение таблицы
    for (int i = 0; i < rows * columns; i++)
    {
        table.SetCellProperties(i, defaultProp);
        table.InsertText(i, 0, "Ячейка " + i);
    }
    
    mt.EndEdit();
    document.EndChanges();
}
```

### 6.2. Пакетное обновление таблицы

```csharp
public static void BatchUpdateTable(Table table, string[,] data)
{
    Document document = table.Document;
    document.BeginChanges("Пакетное обновление таблицы");
    
    int rows = data.GetLength(0);
    int cols = data.GetLength(1);
    
    // Пакетное обновление данных
    for (int row = 0; row < rows; row++)
    {
        for (int col = 0; col < cols; col++)
        {
            int cellIndex = row * cols + col;
            if (cellIndex < table.CellsCount)
            {
                table.InsertText(cellIndex, 0, data[row, col]);
            }
        }
    }
    
    document.EndChanges();
}
```

## 7. Обработка ошибок

### 7.1. Безопасная работа с таблицами

```csharp
public static void SafeTableOperations()
{
    Document document = TFlex.Application.ActiveDocument;
    
    try
    {
        document.BeginChanges("Безопасные операции с таблицей");
        
        MultilineText mt = new MultilineText(document);
        mt.BeginEdit();
        
        Table.CreationSettings sett = new Table.CreationSettings(2, 2);
        Table table = mt.CreateTable(sett);
        
        // Проверка существования таблицы
        if (table != null)
        {
            // Безопасная вставка текста
            if (table.CellsCount > 0)
            {
                table.InsertText(0, 0, "Безопасный текст");
            }
        }
        
        mt.EndEdit();
        document.EndChanges();
    }
    catch (Exception ex)
    {
        document.CancelChanges();
        Console.WriteLine("Ошибка при работе с таблицей: " + ex.Message);
    }
}
```

### 7.2. Валидация данных таблицы

```csharp
public static bool ValidateTableData(Table table)
{
    // Проверка существования таблицы
    if (table == null)
        return false;
    
    // Проверка количества ячеек
    if (table.CellsCount <= 0)
        return false;
    
    // Проверка корректности размеров
    if (table.ColumnsCount <= 0 || table.RowsCount <= 0)
        return false;
    
    return true;
}
```

Эти продвинутые примеры демонстрируют различные аспекты работы с классом `TFlex.Model.Model2D.Table`, включая создание таблиц с пользовательскими стилями, работу с объединенными ячейками, динамическое изменение размеров, интеграцию с другими объектами, оптимизацию производительности и обработку ошибок.