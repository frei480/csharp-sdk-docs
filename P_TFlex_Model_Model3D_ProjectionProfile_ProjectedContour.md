

Руководство по T-FLEX CAD Open API

# ProjectionProfileProjectedContour - свойство  
  
---  
  
Проецируемый контур

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelContour ProjectedContour { get; set; }
```
```vb
Public Property ProjectedContour As ModelContour
	Get
	Set
```
```cpp
public:
property ModelContour^ ProjectedContour {
	ModelContour^ get ();
	void set (ModelContour^ value);
}
```


#### Значение свойства

[ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)

В настоящей версии в качестве контура можно выбирать только листовой профиль. В остальных случаях профиль строится не будет

#### Ссылки

[ProjectionProfile - ](T_TFlex_Model_Model3D_ProjectionProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)