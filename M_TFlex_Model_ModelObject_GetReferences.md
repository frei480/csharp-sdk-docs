

Руководство по T-FLEX CAD Open API

# ModelObjectGetReferences - метод  
  
---  
**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual IEnumerable<ModelObject> GetReferences(
	int id,
	uint firstIndex
)
```
```vb
Public Overridable Function GetReferences ( 
	id As Integer,
	firstIndex As UInteger
) As IEnumerable(Of ModelObject)
```
```cpp
public:
virtual IEnumerable<ModelObject^>^ GetReferences(
	int id, 
	unsigned int firstIndex
)
```


#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
firstIndex [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    

#### Возвращаемое значение

[IEnumerable](https://learn.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1)[ModelObject](T_TFlex_Model_ModelObject.md)

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)