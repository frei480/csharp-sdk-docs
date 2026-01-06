

Руководство по T-FLEX CAD Open API

# TableInsertText(UInt32, UInt32, String, CharFormat) - метод  
    
Вставка текста с использованием заданного формата символов

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertText(
	uint cell,
	uint position,
	string text,
	CharFormat format
)
```
```vb
Public Sub InsertText ( 
	cell As UInteger,
	position As UInteger,
	text As String,
	format As CharFormat
)
```
```cpp
public:
void InsertText(
	unsigned int cell, 
	unsigned int position, 
	String^ text, 
	CharFormat format
)
```


#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы
position [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер символа относительно начала ячейки, перед которым надо вставить текст
text [String](https://learn.microsoft.com/dotnet/api/system.string)
    Текст
format [CharFormat](T_TFlex_Model_Model2D_CharFormat.md)
    Формат символов

После вставки курсор будет перемещён в конец вставленного текста Параметры выделения фрагмента будут потеряны

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[InsertText - перегрузка](Overload_TFlex_Model_Model2D_Table_InsertText.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)