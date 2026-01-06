

Руководство по T-FLEX CAD Open API

# LinkReplaceParents - метод  
  **Пространство имён:** [TFlex.Model.Circuits](N_TFlex_Model_Circuits.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static bool ReplaceParents(
	Document document,
	List<ModelObject> sourceObjects,
	List<ModelObject> targetObjects
)
```
```vb
Public Shared Function ReplaceParents ( 
	document As Document,
	sourceObjects As List(Of ModelObject),
	targetObjects As List(Of ModelObject)
) As Boolean
```
```cpp
public:
static bool ReplaceParents(
	Document^ document, 
	List<ModelObject^>^ sourceObjects, 
	List<ModelObject^>^ targetObjects
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    
sourceObjects [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[ModelObject](T_TFlex_Model_ModelObject.md)
    
targetObjects [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[ModelObject](T_TFlex_Model_ModelObject.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[Link - ](T_TFlex_Model_Circuits_Link.md)

[TFlex.Model.Circuits - пространство имён](N_TFlex_Model_Circuits.md)