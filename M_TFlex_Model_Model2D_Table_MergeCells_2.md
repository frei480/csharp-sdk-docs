

Руководство по T-FLEX CAD Open API

# TableMergeCells(UInt32, UInt32) - метод  
    
Объединение ячеек, лежащих в прямоугольном фрагменте, заданном диагональю

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void MergeCells(
	uint cell1,
	uint cell2
)
```
```vb
Public Sub MergeCells ( 
	cell1 As UInteger,
	cell2 As UInteger
)
```
```cpp
public:
void MergeCells(
	unsigned int cell1, 
	unsigned int cell2
)
```


#### Параметры

cell1 [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы, которая лежит на концах диагонали прямоугольного фрагмента
cell2 [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы, которая лежит на концах диагонали прямоугольного фрагмента

После объединения курсор будет перемещён в начало образовавшейся ячейки Текст ячеек, находящихся во фрагменте будет также объединён Параметры выделения фрагмента будут потеряны

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[MergeCells - перегрузка](Overload_TFlex_Model_Model2D_Table_MergeCells.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)