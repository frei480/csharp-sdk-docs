

Руководство по T-FLEX CAD Open API

# SplineDataControlPointsDelete - метод  
  
---  
  
Удалить контрольную точку по номеру

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Delete(
	uint index
)
```
```vb
Public Sub Delete ( 
	index As UInteger
)
```
```cpp
public:
void Delete(
	unsigned int index
)
```


#### Параметры

index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер контрольной точки

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат не определён

#### Ссылки

[SplineDataControlPoints - ](T_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)