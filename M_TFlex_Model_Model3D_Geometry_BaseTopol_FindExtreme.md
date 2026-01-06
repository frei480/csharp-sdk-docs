

Руководство по T-FLEX CAD Open API

# BaseTopolFindExtreme - метод  
    
Найти экстремальную точку на элементе в заданном направлении

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Point3D FindExtreme(
	BaseDirection direction1,
	BaseDirection direction2,
	BaseDirection direction3
)
```




#### Параметры

direction1 [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Направление 1
direction2 [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Направление 2
direction3 [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Направление 3

#### Возвращаемое значение

[Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)

Экстремальная точка на элементе ищется в направлении 1. Если решение неоднозначное, то количество экстремальных точек последовательно редуцируется по направлениям 2 и 3

#### Ссылки

[BaseTopol - ](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)