

Руководство по T-FLEX CAD Open API

# ModelEdgeGetPolyline(Double, Double, Double) - метод  
  
---  
  
Полилиния

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Point3D[] GetPolyline(
	double curve_chord_tol,
	double curve_chord_ang,
	double curve_chord_max
)
```
```vb
Public Function GetPolyline ( 
	curve_chord_tol As Double,
	curve_chord_ang As Double,
	curve_chord_max As Double
) As Point3D()
```
```cpp
public:
virtual array<Point3D^>^ GetPolyline(
	double curve_chord_tol, 
	double curve_chord_ang, 
	double curve_chord_max
) sealed
```


#### Параметры

curve_chord_tol [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
curve_chord_ang [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
curve_chord_max [Double](https://learn.microsoft.com/dotnet/api/system.double)
    

#### Возвращаемое значение

[Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)

#### Реализации

[BaseEdgeGetPolyline(Double, Double, Double)](M_TFlex_Model_Model3D_Geometry_BaseEdge_GetPolyline_1.md)

#### Ссылки

[ModelEdge - ](T_TFlex_Model_Model3D_Geometry_ModelEdge.md)

[GetPolyline - перегрузка](Overload_TFlex_Model_Model3D_Geometry_ModelEdge_GetPolyline.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)