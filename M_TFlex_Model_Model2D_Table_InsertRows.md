

Руководство по T-FLEX CAD Open API

# TableInsertRows - метод  
  
---  
  
Вставка строк

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertRows(
	uint count,
	uint cell,
	TableInsertProperties props
)
```
```vb
Public Sub InsertRows ( 
	count As UInteger,
	cell As UInteger,
	props As TableInsertProperties
)
```
```cpp
public:
void InsertRows(
	unsigned int count, 
	unsigned int cell, 
	TableInsertProperties props
)
```


#### Параметры

count [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Количество строк
cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы, находящейся в строке, относительно которой надо вставить новые строки
props [TableInsertProperties](T_TFlex_Model_Model2D_Table_InsertProperties.md)
    Параметр вставки

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)