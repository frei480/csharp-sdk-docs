

Руководство по T-FLEX CAD Open API

# EuclideanWorkplaneManagerMovePlane - метод  
    
Переместить рабочую плоскость по нормали к плоскости на заданное значение

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static void MovePlane(
	Workplane plane,
	double offset
)
```
```vb
Public Shared Sub MovePlane ( 
	plane As Workplane,
	offset As Double
)
```
```cpp
public:
static void MovePlane(
	Workplane^ plane, 
	double offset
)
```


#### Параметры

plane [Workplane](T_TFlex_Model_Model3D_Workplane.md)
    Перемещаемая плоскость
offset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Величина, на которую выполняется перемещение

#### Ссылки

[EuclideanWorkplaneManager - ](T_TFlex_Model_Model3D_EuclideanWorkplaneManager.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)