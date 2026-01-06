

Руководство по T-FLEX CAD Open API

# ProjectionPathProjectionSurface - свойство  
    
Поверхность проецирования

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Geometry ProjectionSurface { get; set; }
```
```vb
Public Property ProjectionSurface As Geometry
	Get
	Set
```
```cpp
public:
property Geometry^ ProjectionSurface {
	Geometry^ get ();
	void set (Geometry^ value);
}
```


#### Значение свойства

[Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)

В настоящей версии в качестве поверхности можно выбирать только операции и грани. В остальных случаях путь строится не будет

#### Ссылки

[ProjectionPath - ](T_TFlex_Model_Model3D_ProjectionPath.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)