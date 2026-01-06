

Руководство по T-FLEX CAD Open API

# ConvolutionProfileConvolutionSurface - свойство  
    
Набор граней, образующих поверхность, на которую выполняется свёртка

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FacesArray ConvolutionSurface { get; }
```
```vb
Public ReadOnly Property ConvolutionSurface As FacesArray
	Get
```
```cpp
public:
property FacesArray^ ConvolutionSurface {
	FacesArray^ get ();
}
```


#### Значение свойства

[FacesArray](T_TFlex_Model_Model3D_FacesArray.md)

В настоящей версии в качестве поверхности можно выбирать только конические и цилиндрические грани. В остальных случаях профиль строится не будет. В настоящей версии при свёртке учитываются границы граней. То есть, если границы свёртки пересекают границы грани или не лежат на грани, то профиль строится не будет

#### Ссылки

[ConvolutionProfile - ](T_TFlex_Model_Model3D_ConvolutionProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)