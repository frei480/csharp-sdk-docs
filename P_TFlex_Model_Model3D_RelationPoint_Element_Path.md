

Руководство по T-FLEX CAD Open API

# RelationPointElementPath - свойство  
    
Получить путь, относительно которого или на котором ищется ближайшая точка

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Path3D Path { get; set; }
```
```vb
Public Property Path As Path3D
	Get
	Set
```
```cpp
public:
property Path3D^ Path {
	Path3D^ get ();
	void set (Path3D^ value);
}
```


#### Значение свойства

[Path3D](T_TFlex_Model_Model3D_Path3D.md)

Элемент задаётся несколькими взаимоисключающими способами: гранью, ребром, циклом, путём, операцией. Второй элемент, относительно которого ищется ближайшая точка на первом элементе, может задаваться также точкой

#### Ссылки

[RelationPointElement - ](T_TFlex_Model_Model3D_RelationPoint_Element.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)