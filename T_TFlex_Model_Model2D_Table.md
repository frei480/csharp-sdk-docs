

Руководство по T-FLEX CAD Open API

# Table - структура  
    
Класс для работы с таблицей

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemValueType](https://learn.microsoft.com/dotnet/api/system.valuetype) TFlex.Model.Model2DTable

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public struct Table
```
```vb
Public Structure Table
```
```cpp
public value class Table
```


Тип Table предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [CellCount](P_TFlex_Model_Model2D_Table_CellCount.md) | Количество ячеек |
|  | [ColumnCount](P_TFlex_Model_Model2D_Table_ColumnCount.md) | Количество столбцов. Если в таблице есть разбитые или объединённые ячейки возвращает -1 |
|  | [IsRegular](P_TFlex_Model_Model2D_Table_IsRegular.md) | Количество столбцов строк в таблице неизменно. Если в таблице есть разбитые или объединённые ячейки возвращает false |
|  | [Properties](P_TFlex_Model_Model2D_Table_Properties.md) | Параметры таблицы |
|  | [RowCount](P_TFlex_Model_Model2D_Table_RowCount.md) | Количество строк. Если в таблице есть разбитые или объединённые ячейки возвращает -1 |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clear](M_TFlex_Model_Model2D_Table_Clear.md) | Очистка одержимого ячейки |
|  | [Delete](M_TFlex_Model_Model2D_Table_Delete.md) | Удаление таблицы |
|  | [DeleteColumn](M_TFlex_Model_Model2D_Table_DeleteColumn.md) | Удаление столбца |
|  | [DeleteRow](M_TFlex_Model_Model2D_Table_DeleteRow.md) | Удаление строки |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.valuetype.equals) | Indicates whether this instance and a specified object are equal.(Унаследован от [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)) |
|  | [GetCellData](M_TFlex_Model_Model2D_Table_GetCellData.md) | Получение данных ячейки |
|  | [GetCellHandle](M_TFlex_Model_Model2D_Table_GetCellHandle.md) |  |
|  | [GetCellHeight](M_TFlex_Model_Model2D_Table_GetCellHeight.md) | Получение высоты ячейки |
|  | [GetCellIndex](M_TFlex_Model_Model2D_Table_GetCellIndex.md) |  |
|  | [GetCellProperties](M_TFlex_Model_Model2D_Table_GetCellProperties.md) | Получение параметров ячейки |
|  | [GetCellRectangle](M_TFlex_Model_Model2D_Table_GetCellRectangle.md) | Получение прямоугольника ячейки |
|  | [GetCellsProperties](M_TFlex_Model_Model2D_Table_GetCellsProperties.md) | Получение параметров прямоугольного фрагмента таблицы |
|  | [GetCellText(UInt32)](M_TFlex_Model_Model2D_Table_GetCellText.md) | Получение текста в ячейке |
|  | [GetCellText(UInt32, Boolean)](M_TFlex_Model_Model2D_Table_GetCellText_1.md) | Получение текста в ячейке |
|  | [GetCellTextLength(IntPtr)](M_TFlex_Model_Model2D_Table_GetCellTextLength.md) | Получение количества символов в ячейке |
|  | [GetCellTextLength(UInt32)](M_TFlex_Model_Model2D_Table_GetCellTextLength_1.md) | Получение количества символов в ячейке |
|  | [GetCellTextWithHyperlinks](M_TFlex_Model_Model2D_Table_GetCellTextWithHyperlinks.md) |  |
|  | [GetCellWidth](M_TFlex_Model_Model2D_Table_GetCellWidth.md) | Получение ширины ячейки |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.valuetype.gethashcode) | Returns the hash code for this instance.(Унаследован от [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InsertColumns](M_TFlex_Model_Model2D_Table_InsertColumns.md) | Вставка столбцов |
|  | [InsertRows](M_TFlex_Model_Model2D_Table_InsertRows.md) | Вставка строк |
|  | [InsertText(UInt32, UInt32, String)](M_TFlex_Model_Model2D_Table_InsertText.md) | Вставка текста с использованием формата символа по умолчанию |
|  | [InsertText(UInt32, UInt32, String, CharFormat)](M_TFlex_Model_Model2D_Table_InsertText_1.md) | Вставка текста с использованием заданного формата символов |
|  | [InsertTextWithHyperlinks](M_TFlex_Model_Model2D_Table_InsertTextWithHyperlinks.md) | Вставка текста с использованием формата символа по умолчанию |
|  | [MergeCells](M_TFlex_Model_Model2D_Table_MergeCells.md) | Объединение выделенных ячеек |
|  | [MergeCells(IntPtr, IntPtr)](M_TFlex_Model_Model2D_Table_MergeCells_1.md) |  |
|  | [MergeCells(UInt32, UInt32)](M_TFlex_Model_Model2D_Table_MergeCells_2.md) | Объединение ячеек, лежащих в прямоугольном фрагменте, заданном диагональю |
|  | [SelectAll](M_TFlex_Model_Model2D_Table_SelectAll.md) | Выделение всей таблицы |
|  | [SetCellData](M_TFlex_Model_Model2D_Table_SetCellData.md) | Выставление данных ячейки |
|  | [SetCellHeight](M_TFlex_Model_Model2D_Table_SetCellHeight.md) | Установка высоты ячейки |
|  | [SetCellProperties](M_TFlex_Model_Model2D_Table_SetCellProperties.md) | Установка параметров ячейки |
|  | [SetCellsProperties](M_TFlex_Model_Model2D_Table_SetCellsProperties.md) | Установка параметров прямоугольного фрагмента таблицы |
|  | [SetCellWidth(UInt32, Double)](M_TFlex_Model_Model2D_Table_SetCellWidth.md) | Установка ширины ячейки |
|  | [SetCellWidth(UInt32, Double, ColumnSizeMode)](M_TFlex_Model_Model2D_Table_SetCellWidth_1.md) | Установка ширины ячейки |
|  | [SetCursorPosition](M_TFlex_Model_Model2D_Table_SetCursorPosition.md) | Установка положения курсора |
|  | [SetSelection(IntPtr, IntPtr)](M_TFlex_Model_Model2D_Table_SetSelection.md) |  |
|  | [SetSelection(UInt32, UInt32)](M_TFlex_Model_Model2D_Table_SetSelection_1.md) | Выделение прямоугольного фрагмента таблицы по заданной диагонали |
|  | [SplitCell](M_TFlex_Model_Model2D_Table_SplitCell.md) | Разбивка ячейки на строки и столбцы |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.valuetype.tostring) | Returns the fully qualified type name of this instance.(Унаследован от [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)) |
      
    
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
    
            tbl.InsertText(9, 0, "старый текст");
            mt.EndEdit();
            document.EndChanges();
    
            document.BeginChanges("_");
            MessageBox.Show("очистка ячейки");
    
            mt.BeginEdit();
            tbl.Clear(9);
            mt.EndEdit();
    
            document.EndChanges();
    
            document.BeginChanges("_");
            MessageBox.Show("вставка нового значения в ячейку");
    
            mt.BeginEdit();
            tbl.InsertText(9, 0, "новый текст");
            mt.EndEdit();
    
            document.EndChanges();
            break;
           }
       }
    
    document.EndChanges();
    }

#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)