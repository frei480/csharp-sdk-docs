

Руководство по T-FLEX CAD Open API

# OperationRayTest(Operation, BasePoint3D, BaseDirection, ListDouble) - метод  
  **Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static bool RayTest(
	Operation operation,
	BasePoint3D rayOrigin,
	BaseDirection rayDir,
	List<double> distances
)
```
```vb
Public Shared Function RayTest ( 
	operation As Operation,
	rayOrigin As BasePoint3D,
	rayDir As BaseDirection,
	distances As List(Of Double)
) As Boolean
```
```cpp
public:
static bool RayTest(
	Operation^ operation, 
	BasePoint3D^ rayOrigin, 
	BaseDirection^ rayDir, 
	List<double>^ distances
)
```


#### Параметры

operation [Operation](T_TFlex_Model_Model3D_Operation.md)
    
rayOrigin [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    
rayDir [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    
distances [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[Double](https://learn.microsoft.com/dotnet/api/system.double)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[Operation - ](T_TFlex_Model_Model3D_Operation.md)

[RayTest - перегрузка](Overload_TFlex_Model_Model3D_Operation_RayTest.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)