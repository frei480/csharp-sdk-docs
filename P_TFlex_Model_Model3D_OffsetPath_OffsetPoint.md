

Руководство по T-FLEX CAD Open API

# OffsetPathOffsetPoint - свойство  
    
Точка, определяющая значение смещения

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D OffsetPoint { get; set; }
```
```vb
Public Property OffsetPoint As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ OffsetPoint {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

В настоящей версии в качестве точки можно выбирать только 3D узел. В остальных случаях путь строится не будет. Значение смещения задаётся двумя взаимоисключающими способами: по точке или по значению

#### Ссылки

[OffsetPath - ](T_TFlex_Model_Model3D_OffsetPath.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)