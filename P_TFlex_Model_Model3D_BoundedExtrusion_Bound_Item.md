

Руководство по T-FLEX CAD Open API

# BoundedExtrusionBoundItem - свойство  
    
Граница выталкивания

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Geometry Item { get; set; }
```




#### Значение свойства

[Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)

Граница выталкивания может задаваться только отступом. В этом случае в качестве границы выталкивания берётся сам контур со смещением, задаваемым значением отступа в направлении выталкивания. В качестве границы выталкивания могут передаваться только грани, поверхности, листовые и твёрдые тела. Остальные типы геометрии игнорируются.

#### Ссылки

[BoundedExtrusionBound - ](T_TFlex_Model_Model3D_BoundedExtrusion_Bound.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)