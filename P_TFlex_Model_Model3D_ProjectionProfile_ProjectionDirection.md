

Руководство по T-FLEX CAD Open API

# ProjectionProfileProjectionDirection - свойство  
  
---  
  
Направление проецирования

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelDirection ProjectionDirection { get; set; }
```
```vb
Public Property ProjectionDirection As ModelDirection
	Get
	Set
```
```cpp
public:
property ModelDirection^ ProjectionDirection {
	ModelDirection^ get ();
	void set (ModelDirection^ value);
}
```


#### Значение свойства

[ModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md)

Направление проецирования задаётся двумя взаимоисключающими методами: двумя точками или направлением. В настоящей версии в качестве направления можно выбирать только оси системы координат. В остальных случаях профиль строится не будет. Если направление не задано, то выполняется проецирование по нормали к поверхности

#### Ссылки

[ProjectionProfile - ](T_TFlex_Model_Model3D_ProjectionProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)