

Руководство по T-FLEX CAD Open API

# ConeSurface - конструктор  
    
Создание цилиндра

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ConeSurface(
	double radius,
	double semiangle,
	BaseAxis axis,
	BaseDirection referencedirection
)
```
```vb
Public Sub New ( 
	radius As Double,
	semiangle As Double,
	axis As BaseAxis,
	referencedirection As BaseDirection
)
```
```cpp
public:
ConeSurface(
	double radius, 
	double semiangle, 
	BaseAxis^ axis, 
	BaseDirection^ referencedirection
)
```


#### Параметры

radius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Радиус основания
semiangle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Половина угла конуса в градусах
axis [BaseAxis](T_TFlex_Model_Model3D_Geometry_BaseAxis.md)
    Ось симметрии
referencedirection [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Полуось основания, от которой откладывается угол

#### Ссылки

[ConeSurface - ](T_TFlex_Model_Model3D_Geometry_ConeSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)