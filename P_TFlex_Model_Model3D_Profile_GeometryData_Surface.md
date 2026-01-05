

Руководство по T-FLEX CAD Open API

# ProfileGeometryDataSurface - свойство  
  
---  
  
Получить поверхность, на которой лежит профиль

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelSurface Surface { get; }
```
```vb
Public ReadOnly Property Surface As ModelSurface
	Get
```
```cpp
public:
property ModelSurface^ Surface {
	ModelSurface^ get ();
}
```


#### Возвращаемое значение

[ModelSurface](T_TFlex_Model_Model3D_Geometry_ModelSurface.md)Объект класса [ModelSurface](T_TFlex_Model_Model3D_Geometry_ModelSurface.md), хранящий поверхность и ссылку на эти геометрические данные профиля

Для профилей, состоящих из нескольких граней или состоящих только из рёбер (проволочные профили), поверхность может быть не определена

#### Ссылки

[ProfileGeometryData - ](T_TFlex_Model_Model3D_Profile_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)