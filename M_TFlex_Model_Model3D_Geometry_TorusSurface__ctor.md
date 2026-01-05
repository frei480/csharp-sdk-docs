

Руководство по T-FLEX CAD Open API

# TorusSurface - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public TorusSurface(
	double minorradius,
	double majorradius,
	BaseAxis axis,
	BaseDirection referencedirection
)
```
```vb
Public Sub New ( 
	minorradius As Double,
	majorradius As Double,
	axis As BaseAxis,
	referencedirection As BaseDirection
)
```
```cpp
public:
TorusSurface(
	double minorradius, 
	double majorradius, 
	BaseAxis^ axis, 
	BaseDirection^ referencedirection
)
```


#### Параметры

minorradius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Малый радиус основания
majorradius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Большой радиус основания
axis [BaseAxis](T_TFlex_Model_Model3D_Geometry_BaseAxis.md)
    Ось симметрии
referencedirection [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Полуось основания, от которой откладывается угол

#### Ссылки

[TorusSurface - ](T_TFlex_Model_Model3D_Geometry_TorusSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)