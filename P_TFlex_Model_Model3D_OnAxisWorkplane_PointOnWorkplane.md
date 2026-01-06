

Руководство по T-FLEX CAD Open API

# OnAxisWorkplanePointOnWorkplane - свойство  
    
Точка, задающая доворот рабочей плоскости

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D PointOnWorkplane { get; set; }
```
```vb
Public Property PointOnWorkplane As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ PointOnWorkplane {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Доворот рабочей плоскости задаётся тремя взаимоисключающими способами : \- точкой, через которую проходит рабочая плоскость; \- параметром угла поворота; \- поверхностью, которой касается рабочая плоскость.

#### Ссылки

[OnAxisWorkplane - ](T_TFlex_Model_Model3D_OnAxisWorkplane.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)