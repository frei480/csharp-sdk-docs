

Руководство по T-FLEX CAD Open API

# ProjectionPathProjectedWire - свойство  
    
Проецируемая провлочная геометрия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Wire ProjectedWire { get; set; }
```
```vb
Public Property ProjectedWire As Wire
	Get
	Set
```
```cpp
public:
property Wire^ ProjectedWire {
	Wire^ get ();
	void set (Wire^ value);
}
```


#### Значение свойства

[Wire](T_TFlex_Model_Model3D_Geometry_Wire.md)

В настоящей версии в качестве проволочной модели можно выбирать только 3D путь. В остальных случаях путь строится не будет

#### Ссылки

[ProjectionPath - ](T_TFlex_Model_Model3D_ProjectionPath.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)