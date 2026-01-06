

Руководство по T-FLEX CAD Open API

# TransformationGroupBaseAddMoveToSurfaceTransf - метод  
    
Добавить трансформацию "Перемещение до плоскости" к группе трансформаций

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddMoveToSurfaceTransf(
	TransformationCoordinate axis,
	ModelSurface surface
)
```
```vb
Public Sub AddMoveToSurfaceTransf ( 
	axis As TransformationCoordinate,
	surface As ModelSurface
)
```
```cpp
public:
void AddMoveToSurfaceTransf(
	TransformationCoordinate axis, 
	ModelSurface^ surface
)
```


#### Параметры

axis [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    ось, вдоль которой производится перемещение
surface [ModelSurface](T_TFlex_Model_Model3D_Geometry_ModelSurface.md)
    плоскость, до которой производится перемещение

#### Ссылки

[TransformationGroupBase - ](T_TFlex_Model_Model3D_TransformationGroupBase.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)