

Руководство по T-FLEX CAD Open API

# BaseSurfaceIntersectCurve - метод  
    
Найти пересечение поверхности с кривой

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public IntersectCurveSurfaceData IntersectCurve(
	BaseCurve curve,
	BaseInterval interval,
	bool havebox,
	BaseBox box
)
```
```vb
Public Function IntersectCurve ( 
	curve As BaseCurve,
	interval As BaseInterval,
	havebox As Boolean,
	box As BaseBox
) As IntersectCurveSurfaceData
```
```cpp
public:
IntersectCurveSurfaceData^ IntersectCurve(
	BaseCurve^ curve, 
	BaseInterval^ interval, 
	bool havebox, 
	BaseBox^ box
)
```


#### Параметры

curve [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)
    Кривая, с которой ищется пересечение
interval [BaseInterval](T_TFlex_Model_Model3D_Geometry_BaseInterval.md)
    Параметрический интервал кривой, на котором ищется пересечение
havebox [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать область поиска пересечений
box [BaseBox](T_TFlex_Model_Model3D_Geometry_BaseBox.md)
    Область поиска пересечений

#### Возвращаемое значение

[IntersectCurveSurfaceData](T_TFlex_Model_Model3D_Geometry_IntersectCurveSurfaceData.md)

#### Ссылки

[BaseSurface - ](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)