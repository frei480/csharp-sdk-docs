

Руководство по T-FLEX CAD Open API

# SpatialWorkSurfaceGeometryDataPoint - свойство  
    
Для сферической и тороидальной поверхностей можно получить точку симметрии

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D Point { get; }
```
```vb
Public ReadOnly Property Point As ModelPoint3D
	Get
```
```cpp
public:
property ModelPoint3D^ Point {
	ModelPoint3D^ get ();
}
```


#### Возвращаемое значение

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)Объект класса TFlex::Model::Model3D::Geometry::Point, хранящий координаты точки и ссылку на эти геометрические данные рабочей поверхности

#### Ссылки

[SpatialWorkSurfaceGeometryData - ](T_TFlex_Model_Model3D_SpatialWorkSurface_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)