

Руководство по T-FLEX CAD Open API

# RichTextCreateTable(TableCreationSettings) - метод  
    
Создание таблицы перед символом, на котором находится курсор

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Table CreateTable(
	TableCreationSettings settings
)
```
```vb
Public Function CreateTable ( 
	settings As TableCreationSettings
) As Table
```
```cpp
public:
Table CreateTable(
	TableCreationSettings settings
)
```


#### Параметры

settings [TableCreationSettings](T_TFlex_Model_Model2D_Table_CreationSettings.md)
    Параметры создания таблицы

#### Возвращаемое значение

[Table](T_TFlex_Model_Model2D_Table.md)Таблица

После создания таблицы, курсор перемещается в начало первой ячейки

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[CreateTable - перегрузка](Overload_TFlex_Model_Model2D_RichText_CreateTable.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)