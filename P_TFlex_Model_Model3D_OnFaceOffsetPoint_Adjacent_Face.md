

Руководство по T-FLEX CAD Open API

# OnFaceOffsetPointAdjacentFace - свойство  
    
Смежная грань, от которой строится смещение

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelFace Face { get; set; }
```
```vb
Public Property Face As ModelFace
	Get
	Set
```
```cpp
public:
property ModelFace^ Face {
	ModelFace^ get ();
	void set (ModelFace^ value);
}
```


#### Значение свойства

[ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)

Смещение задаётся двумя взаимоисключающими способами: смежной гранью или смежным ребром

#### Ссылки

[OnFaceOffsetPointAdjacent - ](T_TFlex_Model_Model3D_OnFaceOffsetPoint_Adjacent.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)