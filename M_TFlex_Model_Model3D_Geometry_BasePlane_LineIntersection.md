

Руководство по T-FLEX CAD Open API

# BasePlaneLineIntersection - метод  
    
Получить пересечение плоскости с прямой

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Point3D LineIntersection(
	Axis line
)
```
```vb
Public Function LineIntersection ( 
	line As Axis
) As Point3D
```
```cpp
public:
Point3D^ LineIntersection(
	Axis^ line
)
```


#### Параметры

line [Axis](T_TFlex_Model_Model3D_Geometry_Axis.md)
    Прямая, с которой ищется пересечение

#### Возвращаемое значение

[Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)

Если прямая не пересекает плоскость, то результат нулевой

#### Ссылки

[BasePlane - ](T_TFlex_Model_Model3D_Geometry_BasePlane.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)