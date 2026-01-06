

Руководство по T-FLEX CAD Open API

# EllipConeCreatorCreate - метод  
  **Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static BaseSurface Create(
	double minorRadius,
	double majorRadius,
	double height,
	double semiangle,
	Point3D api_point,
	Direction normal,
	Direction referencedirection
)
```
```vb
Public Shared Function Create ( 
	minorRadius As Double,
	majorRadius As Double,
	height As Double,
	semiangle As Double,
	api_point As Point3D,
	normal As Direction,
	referencedirection As Direction
) As BaseSurface
```
```cpp
public:
static BaseSurface^ Create(
	double minorRadius, 
	double majorRadius, 
	double height, 
	double semiangle, 
	Point3D^ api_point, 
	Direction^ normal, 
	Direction^ referencedirection
)
```


#### Параметры

minorRadius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
majorRadius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
height [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
semiangle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
api_point [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    
normal [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
referencedirection [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    

#### Возвращаемое значение

[BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)

#### Ссылки

[EllipConeCreator - ](T_TFlex_Model_Model3D_Geometry_EllipConeCreator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)