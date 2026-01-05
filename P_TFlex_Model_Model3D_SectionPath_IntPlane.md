

Руководство по T-FLEX CAD Open API

# SectionPathIntPlane - свойство  
  
---  
  
Поверхность

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPlane IntPlane { get; set; }
```
```vb
Public Property IntPlane As ModelPlane
	Get
	Set
```
```cpp
public:
property ModelPlane^ IntPlane {
	ModelPlane^ get ();
	void set (ModelPlane^ value);
}
```


#### Значение свойства

[ModelPlane](T_TFlex_Model_Model3D_Geometry_ModelPlane.md)

В настоящей версии в качестве поверхности можно выбирать только рабочую плоскость. В остальных случаях путь строится не будет

#### Ссылки

[SectionPath - ](T_TFlex_Model_Model3D_SectionPath.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)