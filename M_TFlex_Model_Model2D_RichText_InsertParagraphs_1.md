

Руководство по T-FLEX CAD Open API

# RichTextInsertParagraphs(UInt32, CharFormat) - метод  
    
Вставка нескольких абзацев с использованием для разделителя заданного формата символов

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertParagraphs(
	uint count,
	CharFormat format
)
```




#### Параметры

count [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Количество абзацев
format [CharFormat](T_TFlex_Model_Model2D_CharFormat.md)
    Формат разделителя

Абзацы будет вставлены перед символом, на котором находится курсор. Параметры выделения фрагмента будут потеряны

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[InsertParagraphs - перегрузка](Overload_TFlex_Model_Model2D_RichText_InsertParagraphs.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)