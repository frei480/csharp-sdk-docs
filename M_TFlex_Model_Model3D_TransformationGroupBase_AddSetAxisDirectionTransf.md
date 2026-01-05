

Руководство по T-FLEX CAD Open API

# TransformationGroupBaseAddSetAxisDirectionTransf - метод  
  
---  
  
Добавить трансформацию "Повернуть параллельно направлению" к группе трансформаций.

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddSetAxisDirectionTransf(
	TransformationCoordinate axis,
	ModelDirection direction
)
```
```vb
Public Sub AddSetAxisDirectionTransf ( 
	axis As TransformationCoordinate,
	direction As ModelDirection
)
```
```cpp
public:
void AddSetAxisDirectionTransf(
	TransformationCoordinate axis, 
	ModelDirection^ direction
)
```


#### Параметры

axis [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    Поворачиваемая ось
direction [ModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md)
    Направление, с которым должна совпасть ось

#### Ссылки

[TransformationGroupBase - ](T_TFlex_Model_Model3D_TransformationGroupBase.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)