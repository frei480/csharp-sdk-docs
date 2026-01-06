

Руководство по T-FLEX CAD Open API

# TransformationGroupBaseAddDirectAxisByAxisToDirectionTransf - метод  
    
Добавить трансформацию "Повернуть ось вокруг оси по направлению" к группе трансформаций.

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddDirectAxisByAxisToDirectionTransf(
	TransformationCoordinate stationaryAxis,
	TransformationCoordinate rotatingAxis,
	ModelDirection direction
)
```




#### Параметры

stationaryAxis [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    неподвижная ось
rotatingAxis [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    направляемая ось
direction [ModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md)
    направление для rotatingAxis

#### Ссылки

[TransformationGroupBase - ](T_TFlex_Model_Model3D_TransformationGroupBase.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)