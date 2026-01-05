

Руководство по T-FLEX CAD Open API

# Model3DWorkplaneReferenceDirection - свойство  
  
---  
  
Точка, задающая направление оси X рабочей плоскости

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D ReferenceDirection { get; set; }
```
```vb
Public Property ReferenceDirection As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ ReferenceDirection {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Если не задано начало координат рабочей плоскости, то точка, задающая направление оси X рабочей плоскости, не используется

#### Ссылки

[Model3DWorkplane - ](T_TFlex_Model_Model3D_Model3DWorkplane.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)