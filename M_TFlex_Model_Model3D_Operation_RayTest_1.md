

Руководство по T-FLEX CAD Open API

# OperationRayTest(Operation, ValueType, ValueType, Point3D, Double) - метод  
  
---  
**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static bool RayTest(
	Operation operation,
	ValueType rayOrigin,
	ValueType rayDir,
	ref Point3D intersection,
	ref double distance
)
```
```vb
Public Shared Function RayTest ( 
	operation As Operation,
	rayOrigin As ValueType,
	rayDir As ValueType,
	ByRef intersection As Point3D,
	ByRef distance As Double
) As Boolean
```
```cpp
public:
static bool RayTest(
	Operation^ operation, 
	ValueType^ rayOrigin, 
	ValueType^ rayDir, 
	Point3D^% intersection, 
	double% distance
)
```


#### Параметры

operation [Operation](T_TFlex_Model_Model3D_Operation.md)
    
rayOrigin [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)
    
rayDir [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)
    
intersection [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    
distance [Double](https://learn.microsoft.com/dotnet/api/system.double)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[Operation - ](T_TFlex_Model_Model3D_Operation.md)

[RayTest - перегрузка](Overload_TFlex_Model_Model3D_Operation_RayTest.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)