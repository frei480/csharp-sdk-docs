

Руководство по T-FLEX CAD Open API

# ProjectionGetProjectedPoint - метод  
  
---  
  
Функция возвращает 3D точку по точке на проекции

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Point3D GetProjectedPoint(
	Point3D point
)
```
```vb
Public Function GetProjectedPoint ( 
	point As Point3D
) As Point3D
```
```cpp
public:
Point3D^ GetProjectedPoint(
	Point3D^ point
)
```


#### Параметры

point [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    

#### Возвращаемое значение

[Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)Функция возвращает NULL когда проекция не рассчитана

#### Ссылки

[Projection - ](T_TFlex_Model_Model3D_Projection.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)