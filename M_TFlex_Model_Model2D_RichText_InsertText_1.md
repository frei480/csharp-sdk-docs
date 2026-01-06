

Руководство по T-FLEX CAD Open API

# RichTextInsertText(String, CharFormat) - метод  
    
Вставка текста с использованием заданного формата символов

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertText(
	string text,
	CharFormat format
)
```
```vb
Public Sub InsertText ( 
	text As String,
	format As CharFormat
)
```
```cpp
public:
void InsertText(
	String^ text, 
	CharFormat format
)
```


#### Параметры

text [String](https://learn.microsoft.com/dotnet/api/system.string)
    Текст
format [CharFormat](T_TFlex_Model_Model2D_CharFormat.md)
    Формат символов

Текст будет вставлен перед символом, на котором находится курсор. Параметры выделения фрагмента будут потеряны

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[InsertText - перегрузка](Overload_TFlex_Model_Model2D_RichText_InsertText.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)