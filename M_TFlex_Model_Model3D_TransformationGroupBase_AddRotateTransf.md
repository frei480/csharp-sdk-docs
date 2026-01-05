

Руководство по T-FLEX CAD Open API

# TransformationGroupBaseAddRotateTransf - метод  
  
---  
  
Добавить трансформацию "Вращение" к группе трансформаций

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddRotateTransf(
	TransformationCoordinate direction,
	Parameter angle
)
```
```vb
Public Sub AddRotateTransf ( 
	direction As TransformationCoordinate,
	angle As Parameter
)
```
```cpp
public:
void AddRotateTransf(
	TransformationCoordinate direction, 
	Parameter^ angle
)
```


#### Параметры

direction [TransformationCoordinate](T_TFlex_Model_Model3D_TransformationCoordinate.md)
    ось, вокруг которой производится вращение
angle [Parameter](T_TFlex_Model_Parameter.md)
    угл вращения

#### Ссылки

[TransformationGroupBase - ](T_TFlex_Model_Model3D_TransformationGroupBase.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)