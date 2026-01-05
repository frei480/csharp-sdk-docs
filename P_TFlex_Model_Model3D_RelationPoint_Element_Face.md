

Руководство по T-FLEX CAD Open API

# RelationPointElementFace - свойство  
  
---  
  
Получить грань, относительно которой или на которой ищется ближайшая точка

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

Элемент задаётся несколькими взаимоисключающими способами: гранью, ребром, циклом, путём, операцией. Второй элемент, относительно которого ищется ближайшая точка на первом элементе, может задаваться также точкой

#### Ссылки

[RelationPointElement - ](T_TFlex_Model_Model3D_RelationPoint_Element.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)