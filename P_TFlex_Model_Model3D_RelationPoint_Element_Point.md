

Руководство по T-FLEX CAD Open API

# RelationPointElementPoint - свойство  
    
Второй элемент как точка, относительно которой ищется ближайшая точка на первом элементе

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D Point { get; set; }
```
```vb
Public Property Point As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ Point {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Второй элемент задаётся несколькими взаимоисключающими способами: гранью, ребром, циклом, путём, операцией, точкой. Для первого элемента, на котором ищется точка, это свойство игнорируется

#### Ссылки

[RelationPointElement - ](T_TFlex_Model_Model3D_RelationPoint_Element.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)