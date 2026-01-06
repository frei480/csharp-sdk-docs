

Руководство по T-FLEX CAD Open API

# BaseAxisLineNearPoints - метод  
    
Получить точку на прямой, ближайшую к другой прямой

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Point3D LineNearPoints(
	Axis line
)
```
```vb
Public Function LineNearPoints ( 
	line As Axis
) As Point3D
```
```cpp
public:
Point3D^ LineNearPoints(
	Axis^ line
)
```


#### Параметры

line [Axis](T_TFlex_Model_Model3D_Geometry_Axis.md)
    Ближайшая к данной прямой прямая

#### Возвращаемое значение

[Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)

Если прямые параллельны, то результат нулевой

#### Ссылки

[BaseAxis - ](T_TFlex_Model_Model3D_Geometry_BaseAxis.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)