

Руководство по T-FLEX CAD Open API

# TableInsertText(UInt32, UInt32, String) - метод  
    
Вставка текста с использованием формата символа по умолчанию

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertText(
	uint cell,
	uint position,
	string text
)
```




#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы
position [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер символа относительно начала ячейки, перед которым надо вставить текст
text [String](https://learn.microsoft.com/dotnet/api/system.string)
    Текст

После вставки курсор будет перемещён в конец вставленного текста Параметры выделения фрагмента будут потеряны

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[InsertText - перегрузка](Overload_TFlex_Model_Model2D_Table_InsertText.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)