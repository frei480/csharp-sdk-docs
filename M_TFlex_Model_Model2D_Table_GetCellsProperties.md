

Руководство по T-FLEX CAD Open API

# TableGetCellsProperties - метод  
    
Получение параметров прямоугольного фрагмента таблицы

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public TableCellProperties GetCellsProperties(
	uint cell1,
	uint cell2
)
```




#### Параметры

cell1 [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы, которая лежит на концах диагонали прямоугольного фрагмента
cell2 [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы, которая лежит на концах диагонали прямоугольного фрагмента

#### Возвращаемое значение

[TableCellProperties](T_TFlex_Model_Model2D_Table_CellProperties.md)Параметры прямоугольного фрагмента таблицы

Курсор будет перемещён в начало левой верхней ячейки таблицы. Параметры выделения фрагмента будут потеряны

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)