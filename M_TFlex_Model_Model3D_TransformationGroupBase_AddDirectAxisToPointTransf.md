

Руководство по T-FLEX CAD Open API

# TransformationGroupBaseAddDirectAxisToPointTransf - метод  
    
Добавить трансформацию "Направить ось на точку" к группе трансформаций.

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddDirectAxisToPointTransf(
	TransformationCoordinate axis,
	ModelPoint3D point
)
```
```vb
Public Sub AddDirectAxisToPointTransf ( 
	axis As TransformationCoordinate,
	point As ModelPoint3D
)
```
```cpp
public:
void AddDirectAxisToPointTransf(
	TransformationCoordinate axis, 
	ModelPoint3D^ point
)
```


#### Параметры

axis [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    направляемая ось
point [ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)
    точка, на которую направляется ось

#### Ссылки

[TransformationGroupBase - ](T_TFlex_Model_Model3D_TransformationGroupBase.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)