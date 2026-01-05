

Руководство по T-FLEX CAD Open API

# EuclideanWorkplaneManagerSetDistance - метод  
  
---  
  
Задать расстояние между рабочими плоскостями

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static void SetDistance(
	Workplane basePlane,
	Workplane moveablePlane,
	double dDistance
)
```
```vb
Public Shared Sub SetDistance ( 
	basePlane As Workplane,
	moveablePlane As Workplane,
	dDistance As Double
)
```
```cpp
public:
static void SetDistance(
	Workplane^ basePlane, 
	Workplane^ moveablePlane, 
	double dDistance
)
```


#### Параметры

basePlane [Workplane](T_TFlex_Model_Model3D_Workplane.md)
    Базовая плоскость
moveablePlane [Workplane](T_TFlex_Model_Model3D_Workplane.md)
    Перемещаемая плоскость
dDistance [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Расстояние

#### Ссылки

[EuclideanWorkplaneManager - ](T_TFlex_Model_Model3D_EuclideanWorkplaneManager.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)