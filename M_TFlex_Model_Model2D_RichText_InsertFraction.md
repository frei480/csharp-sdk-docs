

Руководство по T-FLEX CAD Open API

# RichTextInsertFraction - метод  
  
---  
  
Вставка дроби

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertFraction(
	string upper,
	string lower
)
```
```vb
Public Sub InsertFraction ( 
	upper As String,
	lower As String
)
```
```cpp
public:
void InsertFraction(
	String^ upper, 
	String^ lower
)
```


#### Параметры

upper [String](https://learn.microsoft.com/dotnet/api/system.string)
    Строка числителя (может отсутствовать)
lower [String](https://learn.microsoft.com/dotnet/api/system.string)
    Строка знаменателя (может отсутствовать)

При создании дроби используется значение масштаба шрифта, указанное в свойстве [CurrFractionScale](P_TFlex_Model_Model2D_RichText_CurrFractionScale.md)

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)