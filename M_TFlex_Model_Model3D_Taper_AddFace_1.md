

Руководство по T-FLEX CAD Open API

# TaperAddFace(ModelFace, ModelFace) - метод  
    
Добавить пару опорная грань - уклоняемая грань

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddFace(
	ModelFace referenceFace,
	ModelFace draftFace
)
```




#### Параметры

referenceFace [ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)
    Грань используемая в качестве опоры для поворота уклоняемой грани
draftFace [ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)
    Уклоняемая грань

Грани должны иметь общее ребро

#### Ссылки

[Taper - ](T_TFlex_Model_Model3D_Taper.md)

[AddFace - перегрузка](Overload_TFlex_Model_Model3D_Taper_AddFace.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)