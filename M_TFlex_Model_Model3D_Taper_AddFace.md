

Руководство по T-FLEX CAD Open API

# TaperAddFace(ModelEdge, ModelFace) - метод  
    
Добавить пару опорное ребро - уклоняемая грань

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddFace(
	ModelEdge referenceEdge,
	ModelFace draftFace
)
```
```vb
Public Sub AddFace ( 
	referenceEdge As ModelEdge,
	draftFace As ModelFace
)
```
```cpp
public:
void AddFace(
	ModelEdge^ referenceEdge, 
	ModelFace^ draftFace
)
```


#### Параметры

referenceEdge [ModelEdge](T_TFlex_Model_Model3D_Geometry_ModelEdge.md)
    Ребро используемое в качестве опоры для поворота уклоняемой грани
draftFace [ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)
    Уклоняемая грань

Ребро должно принадлежать уклоняемой грани

#### Ссылки

[Taper - ](T_TFlex_Model_Model3D_Taper.md)

[AddFace - перегрузка](Overload_TFlex_Model_Model3D_Taper_AddFace.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)