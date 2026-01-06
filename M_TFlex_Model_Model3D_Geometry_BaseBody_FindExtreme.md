

Руководство по T-FLEX CAD Open API

# BaseBodyFindExtreme - метод  
    
Найти экстремальную точку на теле в заданном направлении

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Point3D FindExtreme(
	BaseDirection direction1,
	BaseDirection direction2,
	BaseDirection direction3
)
```
```vb
Public Function FindExtreme ( 
	direction1 As BaseDirection,
	direction2 As BaseDirection,
	direction3 As BaseDirection
) As Point3D
```
```cpp
public:
Point3D^ FindExtreme(
	BaseDirection^ direction1, 
	BaseDirection^ direction2, 
	BaseDirection^ direction3
)
```


#### Параметры

direction1 [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Первое направление поиска
direction2 [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Второе направление поиска
direction3 [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Третье направление поиска

#### Возвращаемое значение

[Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)

Экстремальная точка ищется в направлении 1. Если решение неоднозначное, то количество экстремальных точек последовательно редуцируется по направлениям 2 и 3. Все три направления взаимно ортогональны

#### Ссылки

[BaseBody - ](T_TFlex_Model_Model3D_Geometry_BaseBody.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)