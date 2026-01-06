

Руководство по T-FLEX CAD Open API

# BaseCurveInterval - метод  
    
Вычислить параметрический интервал на кривой, ограниченный двумя точками, лежащими на кривой

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public BaseInterval Interval(
	BasePoint3D point1,
	BasePoint3D point2
)
```
```vb
Public Function Interval ( 
	point1 As BasePoint3D,
	point2 As BasePoint3D
) As BaseInterval
```
```cpp
public:
BaseInterval^ Interval(
	BasePoint3D^ point1, 
	BasePoint3D^ point2
)
```


#### Параметры

point1 [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    Первая точка на кривой
point2 [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    Вторая точка на кривой

#### Возвращаемое значение

[BaseInterval](T_TFlex_Model_Model3D_Geometry_BaseInterval.md)

#### Ссылки

[BaseCurve - ](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)