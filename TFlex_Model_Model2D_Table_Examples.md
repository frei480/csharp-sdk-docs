# Примеры использования класса TFlex.Model.Model2D.Table

## 1. Создание таблицы

### 1.1. Создание таблицы с использованием TableCreationSettings

```csharp
// Создание настроек для таблицы (7 столбцов, 2 строки)
Table.CreationSettings sett = new Table.CreationSettings(7, 2);

// Создание таблицы
Table table = multilineText.CreateTable(sett);
```

### 1.2. Создание таблицы с пользовательскими свойствами ячеек

```csharp
// Создание настроек для таблицы
Table.CreationSettings sett = new Table.CreationSettings(7, 2);

// Создание свойств ячейки
Table.CellProperties prop = new Table.CellProperties();
prop.TextDirection = Table.TextDirection.BottomToTop;
prop.CellWidth = 20;
prop.RowHeight = 50; 
prop.RowHeightMode = SizeMode.Auto;
prop.RowWrap = false;
prop.CellTextVAlign = Table.TextVAlign.Center;
prop.TableHAlign = Table.TableHAlign.Center;

// Создание таблицы с пользовательскими свойствами ячеек
Table table = multilineText.CreateTable(sett, prop);
```

## 2. Работа с ячейками таблицы

### 2.1. Получение и установка свойств ячейки

```csharp
// Получение свойств ячейки
Table.CellProperties prop = table.GetCellProperties(0);

// Изменение свойств ячейки
prop.CellWidth = 30;
prop.CellTextVAlign = Table.TextVAlign.Top;

// Установка свойств ячейки
table.SetCellProperties(0, prop);
```

### 2.2. Вставка текста в ячейку

```csharp
// Вставка текста в ячейку с использованием формата по умолчанию
table.InsertText(0, 0, "Текст в ячейке");

// Создание пользовательского формата текста
CharFormat format = new CharFormat();
format.FontName = "Arial";
format.FontSize = 12;
format.isBold = true;

// Вставка текста в ячейку с пользовательским форматом
table.InsertText(0, 0, "Текст в ячейке", format);
```

### 2.3. Получение текста из ячейки

```csharp
// Получение текста из ячейки
string text = table.GetCellText(0);

// Получение текста из ячейки с символами форматирования
string textWithBraces = table.GetCellText(0, true);
```

## 3. Управление строками и столбцами

### 3.1. Вставка строк

```csharp
// Вставка 2 строк после строки, содержащей ячейку с индексом 1
table.InsertRows(2, 1, Table.InsertProperties.After);
```

### 3.2. Вставка столбцов

```csharp
// Вставка 2 столбцов после столбца, содержащего ячейку с индексом 1
table.InsertColumns(2, 1, Table.InsertProperties.After);
```

### 3.3. Удаление строки

```csharp
// Удаление строки, содержащей ячейку с индексом 1
table.DeleteRow(1);
```

### 3.4. Удаление столбца

```csharp
// Удаление столбца, содержащего ячейку с индексом 1
table.DeleteColumn(1);
```

## 4. Работа с размерами ячеек

### 4.1. Установка ширины ячейки

```csharp
// Установка ширины ячейки (и всего столбца) в 50 единиц
table.SetCellWidth(0, 50);
```

### 4.2. Получение ширины ячейки

```csharp
// Получение ширины ячейки
double width = table.GetCellWidth(0);
```

### 4.3. Установка высоты ячейки

```csharp
// Установка высоты ячейки (и всей строки) в 30 единиц
table.SetCellHeight(0, 30, SizeMode.Exact);
```

### 4.4. Получение высоты ячейки

```csharp
// Получение высоты ячейки
double height = table.GetCellHeight(0);
```

## 5. Объединение и разделение ячеек

### 5.1. Объединение ячеек

```csharp
// Объединение ячеек с индексами 0 и 1
table.MergeCells(0, 1);
```

### 5.2. Разделение ячейки

```csharp
// Разделение ячейки с индексом 0 на 2 строки и 3 столбца
table.SplitCell(0, 2, 3);
```

## 6. Полный пример создания и заполнения таблицы

```csharp
public static void CreateTable()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("_");

    MultilineText mt = new MultilineText(document);
    mt.BeginEdit();
    mt.X = 100;
    mt.Y = 200;

    ParaFormat pt = mt.ParagraphFormat;
    pt.HorJustification =  ParaFormat.Just.Center;
    mt.ParagraphFormat = pt;

    mt.InsertText("Таблица штуцеров");
    mt.InsertCommonSymbol(CommonSymbol.LineBreak);

    Table.CreationSettings sett = new Table.CreationSettings(7, 2);
    Table table = mt.CreateTable(sett);

    Table.CellProperties prop = table.Properties;
    prop.TextDirection = Table.TextDirection.BottomToTop;
    prop.CellWidth = 20;
    prop.RowHeight = 50; 
    prop.RowHeightMode = SizeMode.Auto;
    prop.RowWrap = false;
    prop.CellTextVAlign = Table.TextVAlign.Center;
    prop.TableHAlign = Table.TableHAlign.Center;
    prop.HalfCellSpace.Horizontal = 0;
    prop.HalfCellSpace.Vertical = 0;

    table.SetCellHeight(0, 300, SizeMode.Exact);

    table.SetCellProperties(0, prop);
    table.InsertText(0, 0, "Обозначение");

    prop.TextDirection = Table.TextDirection.Normal;
    prop.CellWidth = 70;
    table.SetCellProperties(1, prop);
    table.InsertText(1, 0, "Назначение штуцеров");

    prop.CellWidth = 15;
    table.SetCellProperties(2, prop);
    table.InsertText(2, 0, "Кол.");

    table.SetCellProperties(3, prop);
    table.InsertText(3, 0, "DN, мм");
    table.InsertText(4, 0, "PN");

    prop.CellWidth = 34;
    table.SetCellProperties(6, prop);
    table.InsertText(6, 0, "Примечание");

    table.MergeCells(4, 5);

    table.MergeCells(0, 6);
    table.MergeCells(1, 6);
    table.MergeCells(2, 6);
    table.MergeCells(3, 6);

    prop.CellWidth = 20;
    table.SetCellProperties(6, prop);
    table.InsertText(6, 0, "МПа");

    table.SetCellProperties(7, prop);
    table.InsertText(7, 0, "кгc/с м");

    mt.InsertIndex("2", "");

    CharFormat cf =table.CharFormat;
    cf.VertOffset = 30;
    table.InsertText(7, 0, "2", cf);

    table.MergeCells(5, 8);

    mt.EndEdit();    
    document.EndChanges();
}
```

## 7. Пример изменения содержимого существующей таблицы

```csharp
public static void GetTable()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("_");

    foreach(var n in document.GetObjects())
    {
        if (n is MultilineText)
        {
            MultilineText mt = (MultilineText)n;
            mt.BeginEdit();

            Table tbl = (Table)mt.GetFirstTable();
            Table.CellProperties prop = tbl.GetCellProperties(1);

            tbl.InsertRows(1, 7, Table.InsertProperties.After); 
            tbl.InsertText(8, 0, "1");

            tbl.InsertText(9, 0, "старый текст");
            mt.EndEdit();
            document.EndChanges();

            document.BeginChanges("_");
            MessageBox.Show("очистка ячейки");

            mt.BeginEdit();
            tbl.Clear(9);
            mt.EndEdit();

            document.EndChanges();

            document.BeginChanges("_");
            MessageBox.Show("вставка нового значения в ячейку");

            mt.BeginEdit();
            tbl.InsertText(9, 0, "новый текст");
            mt.EndEdit();

            document.EndChanges();
            break;
        }
    }

    document.EndChanges();
}