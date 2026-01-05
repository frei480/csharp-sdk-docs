

Руководство по T-FLEX CAD Open API

# TransformationGroupBaseAddMoveTransf - метод  
  
---  
  
Добавить трансформацию "Перемещение" к группе трансформаций

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddMoveTransf(
	TransformationCoordinate direction,
	Parameter offset
)
```
```vb
Public Sub AddMoveTransf ( 
	direction As TransformationCoordinate,
	offset As Parameter
)
```
```cpp
public:
void AddMoveTransf(
	TransformationCoordinate direction, 
	Parameter^ offset
)
```


#### Параметры

direction [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    Ось, по которой производится перемещение
offset [Parameter](T_TFlex_Model_Parameter.md)
    отступ перемещения

#### Ссылки

[TransformationGroupBase - ](T_TFlex_Model_Model3D_TransformationGroupBase.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)