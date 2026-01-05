

Руководство по T-FLEX CAD Open API

# FaceIntersectCurve - метод  
  
---  
  
Ищет пересечения между указываемым участком кривой и гранью.

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FaceCurveIntersectionData IntersectCurve(
	BaseCurve curve,
	double IntervalStart,
	double IntervalEnd
)
```
```vb
Public Function IntersectCurve ( 
	curve As BaseCurve,
	IntervalStart As Double,
	IntervalEnd As Double
) As FaceCurveIntersectionData
```
```cpp
public:
virtual FaceCurveIntersectionData^ IntersectCurve(
	BaseCurve^ curve, 
	double IntervalStart, 
	double IntervalEnd
) sealed
```


#### Параметры

curve [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)
    Изгиб, с которым будет искаться пересечение
IntervalStart [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Начало интервала изгиба
IntervalEnd [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Конец интервала изгиба

#### Возвращаемое значение

[FaceCurveIntersectionData](T_TFlex_Model_Model3D_Geometry_FaceCurveIntersectionData.md)

#### Ссылки

[Face - ](T_TFlex_Model_Model3D_Geometry_Face.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)