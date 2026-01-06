

Руководство по T-FLEX CAD Open API

# CylinderSurface - конструктор  
    
Конструктор

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public CylinderSurface(
	double radius,
	BaseAxis axis,
	BaseDirection referencedirection
)
```
```vb
Public Sub New ( 
	radius As Double,
	axis As BaseAxis,
	referencedirection As BaseDirection
)
```
```cpp
public:
CylinderSurface(
	double radius, 
	BaseAxis^ axis, 
	BaseDirection^ referencedirection
)
```


#### Параметры

radius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Радиус основания
axis [BaseAxis](T_TFlex_Model_Model3D_Geometry_BaseAxis.md)
    Ось симметрии
referencedirection [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Полуось основания, от которой откладывается угол

#### Ссылки

[CylinderSurface - ](T_TFlex_Model_Model3D_Geometry_CylinderSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)