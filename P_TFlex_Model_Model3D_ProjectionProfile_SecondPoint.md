

Руководство по T-FLEX CAD Open API

# ProjectionProfileSecondPoint - свойство  
    
Вторая точка, задающая направление проецирования

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D SecondPoint { get; set; }
```
```vb
Public Property SecondPoint As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ SecondPoint {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Направление проецирования задаётся двумя взаимоисключающими методами: двумя точками или направлением. В настоящей версии в качестве точки можно выбирать только 3D узлы. В остальных случаях профиль строится не будет. Если направление не задано, то выполняется проецирование по нормали к поверхности

#### Ссылки

[ProjectionProfile - ](T_TFlex_Model_Model3D_ProjectionProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)