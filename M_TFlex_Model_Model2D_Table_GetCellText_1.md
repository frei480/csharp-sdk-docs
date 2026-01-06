

Руководство по T-FLEX CAD Open API

# TableGetCellText(UInt32, Boolean) - метод  
    
Получение текста в ячейке

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public string GetCellText(
	uint cell,
	bool useBraces
)
```
```vb
Public Function GetCellText ( 
	cell As UInteger,
	useBraces As Boolean
) As String
```
```cpp
public:
String^ GetCellText(
	unsigned int cell, 
	bool useBraces
)
```


#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы
useBraces [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает, содержит ли строка символы форматирования

#### Возвращаемое значение

[String](https://learn.microsoft.com/dotnet/api/system.string)Строка с текстом

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[GetCellText - перегрузка](Overload_TFlex_Model_Model2D_Table_GetCellText.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)