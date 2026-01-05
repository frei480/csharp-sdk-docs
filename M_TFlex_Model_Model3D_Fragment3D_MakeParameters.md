

Руководство по T-FLEX CAD Open API

# Fragment3DMakeParameters - метод  
  
---  
**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public List<uint> MakeParameters(
	List<ModelObject> objects,
	bool saveFragmentDocument,
	bool closeFragmentDocument,
	bool regenerateAssembly,
	bool copyConnectorInfo,
	bool associative
)
```
```vb
Public Function MakeParameters ( 
	objects As List(Of ModelObject),
	saveFragmentDocument As Boolean,
	closeFragmentDocument As Boolean,
	regenerateAssembly As Boolean,
	copyConnectorInfo As Boolean,
	associative As Boolean
) As List(Of UInteger)
```
```cpp
public:
List<unsigned int>^ MakeParameters(
	List<ModelObject^>^ objects, 
	bool saveFragmentDocument, 
	bool closeFragmentDocument, 
	bool regenerateAssembly, 
	bool copyConnectorInfo, 
	bool associative
)
```


#### Параметры

objects [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[ModelObject](T_TFlex_Model_ModelObject.md)
    
saveFragmentDocument [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
closeFragmentDocument [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
regenerateAssembly [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
copyConnectorInfo [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
associative [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)

#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)