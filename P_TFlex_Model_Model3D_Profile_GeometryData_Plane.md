

Руководство по T-FLEX CAD Open API

# ProfileGeometryDataPlane - свойство  
  
---  
  
Получить плоскость

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPlane Plane { get; }
```
```vb
Public ReadOnly Property Plane As ModelPlane
	Get
```
```cpp
public:
property ModelPlane^ Plane {
	ModelPlane^ get ();
}
```


#### Возвращаемое значение

[ModelPlane](T_TFlex_Model_Model3D_Geometry_ModelPlane.md)Объект класса [ModelPlane](T_TFlex_Model_Model3D_Geometry_ModelPlane.md), хранящий координаты плоскости и ссылку на эти геометрические данные профиля

Для профилей, состоящих из нескольких граней или одного прямого ребра, плоскость может быть не определена

#### Ссылки

[ProfileGeometryData - ](T_TFlex_Model_Model3D_Profile_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)