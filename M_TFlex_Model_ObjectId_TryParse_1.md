

Руководство по T-FLEX CAD Open API

# ObjectIdTryParse(String, ObjectId) - метод  
    
Распарсить строку в ObjectId. Вернет false, если строка некорректна.

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static bool TryParse(
	string idString,
	out ObjectId id
)
```
```vb
Public Shared Function TryParse ( 
	idString As String,
	<OutAttribute> ByRef id As ObjectId
) As Boolean
```
```cpp
public:
static bool TryParse(
	String^ idString, 
	[OutAttribute] ObjectId^% id
)
```


#### Параметры

idString [String](https://learn.microsoft.com/dotnet/api/system.string)
    
id [ObjectId](T_TFlex_Model_ObjectId.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[ObjectId - ](T_TFlex_Model_ObjectId.md)

[TryParse - перегрузка](Overload_TFlex_Model_ObjectId_TryParse.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)