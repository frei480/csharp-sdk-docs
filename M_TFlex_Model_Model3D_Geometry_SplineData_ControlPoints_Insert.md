

Руководство по T-FLEX CAD Open API

# SplineDataControlPointsInsert - метод  
    
Вставить контрольную точку перед номером

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	uint Index,
	SplineDataControlPointsControlPoint point
)
```




#### Параметры

Index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер контрольной точки
point [SplineDataControlPointsControlPoint](T_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_ControlPoint.md)
    Контрольная точка

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат не определён

#### Ссылки

[SplineDataControlPoints - ](T_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)