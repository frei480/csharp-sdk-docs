

Руководство по T-FLEX CAD Open API

# ModelAttributesGetTextAttributeIfExist - метод  
  
---  
  
Получить значение текстового атрибута

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public string GetTextAttributeIfExist(
	string attribName
)
```
```vb
Public Function GetTextAttributeIfExist ( 
	attribName As String
) As String
```
```cpp
public:
String^ GetTextAttributeIfExist(
	String^ attribName
)
```


#### Параметры

attribName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя атрибута

#### Возвращаемое значение

[String](https://learn.microsoft.com/dotnet/api/system.string)Значение атрибута или null, если атрибута не существует

#### Ссылки

[ModelAttributes - ](T_TFlex_Model_ModelAttributes.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)