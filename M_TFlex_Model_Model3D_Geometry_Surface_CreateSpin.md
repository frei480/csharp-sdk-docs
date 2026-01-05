

Руководство по T-FLEX CAD Open API

# SurfaceCreateSpin - метод  
  
---  
  
Создать поверхность вращения

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Surface CreateSpin(
	BaseCurve curve,
	BaseAxis axis,
	bool simplify,
	bool confine,
	BaseInterval interval
)
```
```vb
Public Shared Function CreateSpin ( 
	curve As BaseCurve,
	axis As BaseAxis,
	simplify As Boolean,
	confine As Boolean,
	interval As BaseInterval
) As Surface
```
```cpp
public:
static Surface^ CreateSpin(
	BaseCurve^ curve, 
	BaseAxis^ axis, 
	bool simplify, 
	bool confine, 
	BaseInterval^ interval
)
```


#### Параметры

curve [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)
    Вращаемая кривая
axis [BaseAxis](T_TFlex_Model_Model3D_Geometry_BaseAxis.md)
    Ось вращения
simplify [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Для результирующей поверхности подбирать аналитическое решение
confine [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Поверхность вращения создаётся только для части кривой, границы которой задаются интервалом
interval [BaseInterval](T_TFlex_Model_Model3D_Geometry_BaseInterval.md)
    Параметрический интервал на кривой, если поверхность вращения создаётся только для части кривой

#### Возвращаемое значение

[Surface](T_TFlex_Model_Model3D_Geometry_Surface.md)

#### Ссылки

[Surface - ](T_TFlex_Model_Model3D_Geometry_Surface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)