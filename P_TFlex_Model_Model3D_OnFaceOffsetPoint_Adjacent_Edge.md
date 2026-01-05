

Руководство по T-FLEX CAD Open API

# OnFaceOffsetPointAdjacentEdge - свойство  
  
---  
  
Смежное ребро, от которого строится смещение

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelEdge Edge { get; set; }
```
```vb
Public Property Edge As ModelEdge
	Get
	Set
```
```cpp
public:
property ModelEdge^ Edge {
	ModelEdge^ get ();
	void set (ModelEdge^ value);
}
```


#### Значение свойства

[ModelEdge](T_TFlex_Model_Model3D_Geometry_ModelEdge.md)

Смещение задаётся двумя взаимоисключающими способами: смежной гранью или смежным ребром

#### Ссылки

[OnFaceOffsetPointAdjacent - ](T_TFlex_Model_Model3D_OnFaceOffsetPoint_Adjacent.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)