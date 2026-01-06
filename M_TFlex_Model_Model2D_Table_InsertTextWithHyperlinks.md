

Руководство по T-FLEX CAD Open API

# TableInsertTextWithHyperlinks - метод  
    
Вставка текста с использованием формата символа по умолчанию

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool InsertTextWithHyperlinks(
	uint cell,
	uint position,
	string text
)
```
```vb
Public Function InsertTextWithHyperlinks ( 
	cell As UInteger,
	position As UInteger,
	text As String
) As Boolean
```
```cpp
public:
bool InsertTextWithHyperlinks(
	unsigned int cell, 
	unsigned int position, 
	String^ text
)
```


#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы
position [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер символа относительно начала ячейки, перед которым надо вставить текст
text [String](https://learn.microsoft.com/dotnet/api/system.string)
    Текст содержащий гиперссылоки аналогичные гиперссылкам в html

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

После вставки курсор будет перемещён в конец вставленного текста Параметры выделения фрагмента будут потеряны Примеры ссылки [SomeText](http://www.awe?23#=)

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)