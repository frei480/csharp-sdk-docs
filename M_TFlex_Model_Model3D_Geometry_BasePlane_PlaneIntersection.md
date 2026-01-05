

Руководство по T-FLEX CAD Open API

# BasePlanePlaneIntersection - метод  
  
---  
  
Получить пересечение двух плоскостей

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Axis PlaneIntersection(
	BasePlane plane
)
```
```vb
Public Function PlaneIntersection ( 
	plane As BasePlane
) As Axis
```
```cpp
public:
Axis^ PlaneIntersection(
	BasePlane^ plane
)
```


#### Параметры

plane [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)
    Плоскость, с которой ищется пересечение

#### Возвращаемое значение

[Axis](T_TFlex_Model_Model3D_Geometry_Axis.md)

Если плоскости параллельны, то результат нулевой

#### Ссылки

[BasePlane - ](T_TFlex_Model_Model3D_Geometry_BasePlane.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)