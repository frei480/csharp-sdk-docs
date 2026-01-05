

Руководство по T-FLEX CAD Open API

# BaseCurveIntersectCurve - метод  
  
---  
  
Найти пересечение кривой с другой кривой

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public IntersectCurveData IntersectCurve(
	BaseInterval owninterval,
	BaseCurve curve,
	BaseInterval interval,
	bool havebox,
	BaseBox box,
	bool havesurface,
	BaseSurface surface
)
```
```vb
Public Function IntersectCurve ( 
	owninterval As BaseInterval,
	curve As BaseCurve,
	interval As BaseInterval,
	havebox As Boolean,
	box As BaseBox,
	havesurface As Boolean,
	surface As BaseSurface
) As IntersectCurveData
```
```cpp
public:
IntersectCurveData^ IntersectCurve(
	BaseInterval^ owninterval, 
	BaseCurve^ curve, 
	BaseInterval^ interval, 
	bool havebox, 
	BaseBox^ box, 
	bool havesurface, 
	BaseSurface^ surface
)
```


#### Параметры

owninterval [BaseInterval](T_TFlex_Model_Model3D_Geometry_BaseInterval.md)
    Собственный параметрический интервал, на котором ищется пересечение
curve [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)
    Кривая, с которой ищется пересечение
interval [BaseInterval](T_TFlex_Model_Model3D_Geometry_BaseInterval.md)
    Параметрический интервал кривой, на котором ищется пересечение
havebox [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать область поиска пересечений
box [BaseBox](T_TFlex_Model_Model3D_Geometry_BaseBox.md)
    Область поиска пересечений
havesurface [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Кривые лежат на одной поверхности
surface [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)
    

#### Возвращаемое значение

[IntersectCurveData](T_TFlex_Model_Model3D_Geometry_IntersectCurveData.md)

#### Ссылки

[BaseCurve - ](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)