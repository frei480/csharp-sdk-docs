

Руководство по T-FLEX CAD Open API

# TableSplitCell - метод  
    
Разбивка ячейки на строки и столбцы

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SplitCell(
	uint cell,
	uint rows,
	uint columns
)
```




#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы
rows [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Количество строк
columns [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Количество столбцов

После разбиения курсор будет перемещён в начало левой верхней ячейки (из образовавшихся), в которую так же будет перенесён весь текст разбиваемой ячейки Параметры выделения фрагмента будут потеряны

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)