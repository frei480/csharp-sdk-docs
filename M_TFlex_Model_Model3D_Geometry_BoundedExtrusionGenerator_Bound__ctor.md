

Руководство по T-FLEX CAD Open API

# BoundedExtrusionGeneratorBound(Boolean, Double) - конструктор  
  
---  
  
Конструктор для задания границы значением отступа

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Bound(
	bool forward,
	double distance
)
```
```vb
Public Sub New ( 
	forward As Boolean,
	distance As Double
)
```
```cpp
public:
Bound(
	bool forward, 
	double distance
)
```


#### Параметры

forward [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Граница задаётся в направлении вектора выталкивания ( true ) или в обратном направлении ( false )
distance [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Расстояние до границы в заданном направлении. Расстояние должно задаваться неотрицательным значением

#### Ссылки

[BoundedExtrusionGeneratorBound - ](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound.md)

[BoundedExtrusionGeneratorBound - перегрузка](Overload_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound__ctor.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)