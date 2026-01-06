

Руководство по T-FLEX CAD Open API

# MeshWorkPlaneFindMinMax - метод  
    
Найти минимальную или максимальную точку на луче

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public MeshPoint FindMinMax(
	Axis axis,
	bool max
)
```
```vb
Public Function FindMinMax ( 
	axis As Axis,
	max As Boolean
) As MeshPoint
```
```cpp
public:
MeshPoint^ FindMinMax(
	Axis^ axis, 
	bool max
)
```


#### Параметры

axis [Axis](T_TFlex_Model_Model3D_Geometry_Axis.md)
    Геометрическая ось
max [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    true, если ищется максимальная точка, в противном случае false

#### Возвращаемое значение

[MeshPoint](T_TFlex_Model_Model3D_MeshPoint.md)

#### Ссылки

[MeshWorkPlane - ](T_TFlex_Model_Model3D_MeshWorkPlane.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)