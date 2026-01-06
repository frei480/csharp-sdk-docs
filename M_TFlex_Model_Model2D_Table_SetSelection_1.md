

Руководство по T-FLEX CAD Open API

# TableSetSelection(UInt32, UInt32) - метод  
    
Выделение прямоугольного фрагмента таблицы по заданной диагонали

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetSelection(
	uint cell1,
	uint cell2
)
```
```vb
Public Sub SetSelection ( 
	cell1 As UInteger,
	cell2 As UInteger
)
```
```cpp
public:
void SetSelection(
	unsigned int cell1, 
	unsigned int cell2
)
```


#### Параметры

cell1 [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы, которая лежат на концах диагонали выделяемого прямоугольного фрагмента
cell2 [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы, которая лежат на концах диагонали выделяемого прямоугольного фрагмента

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[SetSelection - перегрузка](Overload_TFlex_Model_Model2D_Table_SetSelection.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)