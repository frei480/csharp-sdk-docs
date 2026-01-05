

Руководство по T-FLEX CAD Open API

# CylinderDevelopmentProfilePointOnFace - свойство  
  
---  
  
Точка на грани

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D PointOnFace { get; set; }
```
```vb
Public Property PointOnFace As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ PointOnFace {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Эта точка задаёт начало развёртки. В настоящей версии в качестве точки можно выбирать только 3D узлы. В остальных случаях профиль строится не будет

#### Ссылки

[CylinderDevelopmentProfile - ](T_TFlex_Model_Model3D_CylinderDevelopmentProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)