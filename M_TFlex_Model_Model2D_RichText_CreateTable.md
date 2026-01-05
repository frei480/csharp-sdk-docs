

Руководство по T-FLEX CAD Open API

# RichTextCreateTable(UInt32, TableCreationSettings) - метод  
  
---  
  
Создание таблицы перед символом, заданным порядковым номером относительно начала текста

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Table CreateTable(
	uint position,
	TableCreationSettings settings
)
```
```vb
Public Function CreateTable ( 
	position As UInteger,
	settings As TableCreationSettings
) As Table
```
```cpp
public:
Table CreateTable(
	unsigned int position, 
	TableCreationSettings settings
)
```


#### Параметры

position [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер символа, перед которым надо вставить таблицу, относительно начала текста
settings [TableCreationSettings](T_TFlex_Model_Model2D_Table_CreationSettings.md)
    Параметры создания таблицы

#### Возвращаемое значение

[Table](T_TFlex_Model_Model2D_Table.md)Таблица

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[CreateTable - перегрузка](Overload_TFlex_Model_Model2D_RichText_CreateTable.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)