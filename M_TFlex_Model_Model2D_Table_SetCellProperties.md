

Руководство по T-FLEX CAD Open API

# TableSetCellProperties - метод  
  
---  
  
Установка параметров ячейки

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetCellProperties(
	uint cell,
	TableCellProperties props
)
```
```vb
Public Sub SetCellProperties ( 
	cell As UInteger,
	props As TableCellProperties
)
```
```cpp
public:
void SetCellProperties(
	unsigned int cell, 
	TableCellProperties props
)
```


#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы
props [TableCellProperties](T_TFlex_Model_Model2D_Table_CellProperties.md)
    Новые параметры ячейки таблицы

Курсор будет перемещён в начало заданной ячейки таблицы. Параметры выделения фрагмента будут потеряны

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)