

Руководство по T-FLEX CAD Open API

# FilterTryParse - метод  
    
Перобразовывает заданное строковое представление фильтра в эквивалентный ему объект фильтра

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public static bool TryParse(
	string str,
	Term termTemplate,
	out Filter filter
)
```
```vb
Public Shared Function TryParse ( 
	str As String,
	termTemplate As Term,
	<OutAttribute> ByRef filter As Filter
) As Boolean
```
```cpp
public:
static bool TryParse(
	String^ str, 
	Term^ termTemplate, 
	[OutAttribute] Filter^% filter
)
```


#### Параметры

str [String](https://learn.microsoft.com/dotnet/api/system.string)
    Строковое представление фильтра
termTemplate [Term](T_TFlex_Model_Data_Filters_Term.md)
    Шаблонный параметр
filter [Filter](T_TFlex_Model_Data_Filters_Filter.md)
    Фильтр, эквивалентный указанному строковому представлению

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Значение true, если объект фильтра успешно получен; в противном случае - значение false

#### Ссылки

[Filter - ](T_TFlex_Model_Data_Filters_Filter.md)

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)