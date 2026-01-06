

Руководство по T-FLEX CAD Open API

# BoundedExtrusionGeneratorBoundBoundBody - свойство  
    
Граничное тело

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public BaseBody BoundBody { get; set; }
```
```vb
Public Property BoundBody As BaseBody
	Get
	Set
```
```cpp
public:
property BaseBody^ BoundBody {
	BaseBody^ get ();
	void set (BaseBody^ value);
}
```


#### Значение свойства

[BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)

Граница может задаваться четырьмя взаимоисключающими способами : листовым или твёрдым телом, гранью, поверхностью, отступом. Граничное тело можно задавать если выбран тип границы Body или Sheet. Соответсвенно тело должно быть заданного типа.

#### Ссылки

[BoundedExtrusionGeneratorBound - ](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)