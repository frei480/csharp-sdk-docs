

Руководство по T-FLEX CAD Open API

# ModelObjectGetTextProp - метод  
    
**Примечание: Данный API устарел.**

Измеримые свойства объекта

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This method is obsolete and will be removed. Please use 'GetTextProperty' method.")]
public string GetTextProp(
	string prop,
	ref bool exist
)
```
```vb
<ObsoleteAttribute("This method is obsolete and will be removed. Please use 'GetTextProperty' method.")>
Public Function GetTextProp ( 
	prop As String,
	ByRef exist As Boolean
) As String
```
```cpp
public:
[ObsoleteAttribute(L"This method is obsolete and will be removed. Please use 'GetTextProperty' method.")]
String^ GetTextProp(
	String^ prop, 
	bool% exist
)
```


#### Параметры

prop [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя свойства
exist [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак существования такого свойства

#### Возвращаемое значение

[String](https://learn.microsoft.com/dotnet/api/system.string)

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)