

Руководство по T-FLEX CAD Open API

# SectionPathIntSurface - свойство  
  
---  
  
**Примечание: Данный API устарел.**

Поверхность

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute]
public ModelSurface IntSurface { get; set; }
```
```vb
<ObsoleteAttribute>
Public Property IntSurface As ModelSurface
	Get
	Set
```
```cpp
public:
[ObsoleteAttribute]
property ModelSurface^ IntSurface {
	ModelSurface^ get ();
	void set (ModelSurface^ value);
}
```


#### Значение свойства

[ModelSurface](T_TFlex_Model_Model3D_Geometry_ModelSurface.md)

В настоящей версии в качестве поверхности можно выбирать только рабочую плоскость. В остальных случаях путь строится не будет

#### Ссылки

[SectionPath - ](T_TFlex_Model_Model3D_SectionPath.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)