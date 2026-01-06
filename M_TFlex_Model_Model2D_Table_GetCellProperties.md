

Руководство по T-FLEX CAD Open API

# TableGetCellProperties - метод  
    
Получение параметров ячейки

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public TableCellProperties GetCellProperties(
	uint cell
)
```
```vb
Public Function GetCellProperties ( 
	cell As UInteger
) As TableCellProperties
```
```cpp
public:
TableCellProperties GetCellProperties(
	unsigned int cell
)
```


#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы

#### Возвращаемое значение

[TableCellProperties](T_TFlex_Model_Model2D_Table_CellProperties.md)Параметры ячейки таблицы

Курсор будет перемещён в начало заданной ячейки таблицы. Параметры выделения фрагмента будут потеряны

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)