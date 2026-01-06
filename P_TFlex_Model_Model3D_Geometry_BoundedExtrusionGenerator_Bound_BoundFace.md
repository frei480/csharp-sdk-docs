

Руководство по T-FLEX CAD Open API

# BoundedExtrusionGeneratorBoundBoundFace - свойство  
    
Граничная грань

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public BaseFace BoundFace { get; set; }
```
```vb
Public Property BoundFace As BaseFace
	Get
	Set
```
```cpp
public:
property BaseFace^ BoundFace {
	BaseFace^ get ();
	void set (BaseFace^ value);
}
```


#### Значение свойства

[BaseFace](T_TFlex_Model_Model3D_Geometry_BaseFace.md)

Граница может задаваться четырьмя взаимоисключающими способами : листовым или твёрдым телом, гранью, поверхностью, отступом. Граничную грань можно задавать если выбран тип границы Face.

#### Ссылки

[BoundedExtrusionGeneratorBound - ](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)