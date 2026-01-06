

Руководство по T-FLEX CAD Open API

# RichTextInsertCopyOfTable(Table) - метод  
    
Вставка копии таблицы перед символом, на котором находится курсор

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Table InsertCopyOfTable(
	Table table
)
```
```vb
Public Function InsertCopyOfTable ( 
	table As Table
) As Table
```
```cpp
public:
Table InsertCopyOfTable(
	Table table
)
```


#### Параметры

table [Table](T_TFlex_Model_Model2D_Table.md)
    Таблица, копию которой надо создать

#### Возвращаемое значение

[Table](T_TFlex_Model_Model2D_Table.md)Копия таблицы

После создания таблицы, курсор перемещается в начало первой ячейки

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[InsertCopyOfTable - перегрузка](Overload_TFlex_Model_Model2D_RichText_InsertCopyOfTable.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)