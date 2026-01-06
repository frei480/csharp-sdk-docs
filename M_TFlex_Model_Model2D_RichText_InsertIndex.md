

Руководство по T-FLEX CAD Open API

# RichTextInsertIndex - метод  
    
Вставка индексов

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertIndex(
	string upper,
	string lower
)
```
```vb
Public Sub InsertIndex ( 
	upper As String,
	lower As String
)
```
```cpp
public:
void InsertIndex(
	String^ upper, 
	String^ lower
)
```


#### Параметры

upper [String](https://learn.microsoft.com/dotnet/api/system.string)
    Строка в верхнем индексе (может отсутствовать)
lower [String](https://learn.microsoft.com/dotnet/api/system.string)
    Строка в нижнем индексе (может отсутствовать)

При создании индекса используется значение масштаба шрифта, указанное в свойстве [CurrIndexScale](P_TFlex_Model_Model2D_RichText_CurrIndexScale.md)

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)