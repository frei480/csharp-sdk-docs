

Руководство по T-FLEX CAD Open API

# TableSetCellWidth(UInt32, Double, ColumnSizeMode) - метод  
  
---  
  
Установка ширины ячейки

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetCellWidth(
	uint cell,
	double width,
	ColumnSizeMode mode
)
```
```vb
Public Sub SetCellWidth ( 
	cell As UInteger,
	width As Double,
	mode As ColumnSizeMode
)
```
```cpp
public:
void SetCellWidth(
	unsigned int cell, 
	double width, 
	ColumnSizeMode mode
)
```


#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы
width [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Новая ширина ячейки
mode [ColumnSizeMode](T_TFlex_Model_Model2D_ColumnSizeMode.md)
    Режим задания ширины ячейки

Будет изменена ширина всего столбца, содержащего данную ячейку

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[SetCellWidth - перегрузка](Overload_TFlex_Model_Model2D_Table_SetCellWidth.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)