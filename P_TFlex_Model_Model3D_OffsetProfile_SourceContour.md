

Руководство по T-FLEX CAD Open API

# OffsetProfileSourceContour - свойство  
    
Плоский контур, для которого строится смещение

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelContour SourceContour { get; set; }
```
```vb
Public Property SourceContour As ModelContour
	Get
	Set
```
```cpp
public:
property ModelContour^ SourceContour {
	ModelContour^ get ();
	void set (ModelContour^ value);
}
```


#### Значение свойства

[ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)

В настоящей версии в качестве контура можно выбирать только плоские листовые профили. В остальных случаях профиль строится не будет

#### Ссылки

[OffsetProfile - ](T_TFlex_Model_Model3D_OffsetProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)