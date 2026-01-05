

Руководство по T-FLEX CAD Open API

# OnAxisWorkplaneEdgeOnWorkplane - свойство  
  
---  
  
**Примечание: Данный API устарел.**

Плоское ребро, которое лежит на рабочей плоскости

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This property is obsolete and will be removed. Please use 'AxisOnWorkplane' method.")]
public ModelEdge EdgeOnWorkplane { get; set; }
```
```vb
<ObsoleteAttribute("This property is obsolete and will be removed. Please use 'AxisOnWorkplane' method.")>
Public Property EdgeOnWorkplane As ModelEdge
	Get
	Set
```
```cpp
public:
[ObsoleteAttribute(L"This property is obsolete and will be removed. Please use 'AxisOnWorkplane' method.")]
property ModelEdge^ EdgeOnWorkplane {
	ModelEdge^ get ();
	void set (ModelEdge^ value);
}
```


#### Значение свойства

[ModelEdge](T_TFlex_Model_Model3D_Geometry_ModelEdge.md)

Положение рабочей плоскости задаётся двумя взаимоисключающими способами : плоским ребром или осью. Если ребро прямое, то также как и в случае выбора оси можно дополнительно задавать доворот рабочей плоскости относительно оси или ребра

#### Ссылки

[OnAxisWorkplane - ](T_TFlex_Model_Model3D_OnAxisWorkplane.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)