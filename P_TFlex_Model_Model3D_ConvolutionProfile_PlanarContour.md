

Руководство по T-FLEX CAD Open API

# ConvolutionProfilePlanarContour - свойство  
  
---  
  
Сворачиваемый плоский контур

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelContour PlanarContour { get; set; }
```
```vb
Public Property PlanarContour As ModelContour
	Get
	Set
```
```cpp
public:
property ModelContour^ PlanarContour {
	ModelContour^ get ();
	void set (ModelContour^ value);
}
```


#### Значение свойства

[ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)

В настоящей версии в качестве контура можно выбирать только плоские листовые профили. В остальных случаях профиль строится не будет

#### Ссылки

[ConvolutionProfile - ](T_TFlex_Model_Model3D_ConvolutionProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)