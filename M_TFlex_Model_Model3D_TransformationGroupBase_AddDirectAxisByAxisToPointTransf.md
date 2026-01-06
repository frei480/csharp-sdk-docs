

Руководство по T-FLEX CAD Open API

# TransformationGroupBaseAddDirectAxisByAxisToPointTransf - метод  
    
Добавить трансформацию "Повернуть ось вокруг оси по направлению к точке" к группе трансформаций.

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddDirectAxisByAxisToPointTransf(
	TransformationCoordinate stationaryAxis,
	TransformationCoordinate rotatingAxis,
	ModelPoint3D point
)
```




#### Параметры

stationaryAxis [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    неподвижная ось
rotatingAxis [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    направляемая ось
point [ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)
    точка, на которую направляется rotatingAxis ось

#### Ссылки

[TransformationGroupBase - ](T_TFlex_Model_Model3D_TransformationGroupBase.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)