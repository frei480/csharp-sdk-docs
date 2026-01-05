

Руководство по T-FLEX CAD Open API

# FaceBlendingAddLeftFace - метод  
  
---  
  
Добавить грань в левую стенку

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddLeftFace(
	ModelFace face
)
```
```vb
Public Sub AddLeftFace ( 
	face As ModelFace
)
```
```cpp
public:
void AddLeftFace(
	ModelFace^ face
)
```


#### Параметры

face [ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)
    Грань

Все левые грани должны образовывать G1-непрерывную поверхность. Все левые грани должны принадлежать одному телу.

#### Ссылки

[FaceBlending - ](T_TFlex_Model_Model3D_FaceBlending.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)