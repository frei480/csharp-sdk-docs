

Руководство по T-FLEX CAD Open API

# WorkplaneGeometryDataAxis - свойство  
  
---  
  
**Примечание: Данный API устарел.**

Получить ось

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This method is obsolete and will be removed.")]
public ModelAxis Axis { get; }
```
```vb
<ObsoleteAttribute("This method is obsolete and will be removed.")>
Public ReadOnly Property Axis As ModelAxis
	Get
```
```cpp
public:
[ObsoleteAttribute(L"This method is obsolete and will be removed.")]
property ModelAxis^ Axis {
	ModelAxis^ get ();
}
```


#### Возвращаемое значение

[ModelAxis](T_TFlex_Model_Model3D_Geometry_ModelAxis.md)Объект класса TFlex::Model :: Model3D::Geometry::ModelAxis, хранящий координаты оси и ссылку на эти геометрические данные рабочей плоскости

Направление оси задаётся нормалью к плоскости. Ось проходит через нулевую точку плоскости

#### Ссылки

[WorkplaneGeometryData - ](T_TFlex_Model_Model3D_Workplane_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)