

Руководство по T-FLEX CAD Open API

# SpatialWorkSurfaceGeometryDataSheet - свойство  
  
---  
  
Для сферической и тороидальной поверхностей можно получить листовое тело

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelSheet Sheet { get; }
```
```vb
Public ReadOnly Property Sheet As ModelSheet
	Get
```
```cpp
public:
property ModelSheet^ Sheet {
	ModelSheet^ get ();
}
```


#### Возвращаемое значение

[ModelSheet](T_TFlex_Model_Model3D_Geometry_ModelSheet.md)Объект класса TFlex::Model::Model3D::Geometry::Sheet, хранящий листовое тело и ссылку на эти геометрические данные рабочей поверхности

#### Ссылки

[SpatialWorkSurfaceGeometryData - ](T_TFlex_Model_Model3D_SpatialWorkSurface_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)