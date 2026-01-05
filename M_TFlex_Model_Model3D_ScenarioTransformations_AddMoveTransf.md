

Руководство по T-FLEX CAD Open API

# ScenarioTransformationsAddMoveTransf - метод  
  
---  
  
Добавить трансформацию "Перемещение" к группе трансформаций

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddMoveTransf(
	TransformationCoordinate direction,
	double offset
)
```
```vb
Public Sub AddMoveTransf ( 
	direction As TransformationCoordinate,
	offset As Double
)
```
```cpp
public:
void AddMoveTransf(
	TransformationCoordinate direction, 
	double offset
)
```


#### Параметры

direction [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    Ось, по которой производится перемещение
offset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    отступ перемещения

#### Ссылки

[ScenarioTransformations - ](T_TFlex_Model_Model3D_ScenarioTransformations.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)