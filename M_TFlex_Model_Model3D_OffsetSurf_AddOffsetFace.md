

Руководство по T-FLEX CAD Open API

# OffsetSurfAddOffsetFace - метод  
  
---  
  
Добавить грань с особым смещением

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddOffsetFace(
	ModelFace face,
	Parameter offset
)
```
```vb
Public Sub AddOffsetFace ( 
	face As ModelFace,
	offset As Parameter
)
```
```cpp
public:
void AddOffsetFace(
	ModelFace^ face, 
	Parameter^ offset
)
```


#### Параметры

face [ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)
    Грань
offset [Parameter](T_TFlex_Model_Parameter.md)
    Смещение грани

Все грани задаваемые в операции должны быть с одного тела

#### Ссылки

[OffsetSurf - ](T_TFlex_Model_Model3D_OffsetSurf.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)