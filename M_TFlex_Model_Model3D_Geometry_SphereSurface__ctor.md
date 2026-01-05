

Руководство по T-FLEX CAD Open API

# SphereSurface - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SphereSurface(
	double radius,
	BasePoint3D center,
	BaseDirection normal,
	BaseDirection referencedirection
)
```
```vb
Public Sub New ( 
	radius As Double,
	center As BasePoint3D,
	normal As BaseDirection,
	referencedirection As BaseDirection
)
```
```cpp
public:
SphereSurface(
	double radius, 
	BasePoint3D^ center, 
	BaseDirection^ normal, 
	BaseDirection^ referencedirection
)
```


#### Параметры

radius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
center [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    Радиус сферы
normal [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Ось симметрии
referencedirection [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Полуось основания, от которой откладывается угол

#### Ссылки

[SphereSurface - ](T_TFlex_Model_Model3D_Geometry_SphereSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)