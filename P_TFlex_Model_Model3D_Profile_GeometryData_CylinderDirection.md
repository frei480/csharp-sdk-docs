

Руководство по T-FLEX CAD Open API

# ProfileGeometryDataCylinderDirection - свойство  
  
---  
  
Если профиль лежит на цилиндре, то можно получить направление его оси

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelDirection CylinderDirection { get; }
```
```vb
Public ReadOnly Property CylinderDirection As ModelDirection
	Get
```
```cpp
public:
property ModelDirection^ CylinderDirection {
	ModelDirection^ get ();
}
```


#### Возвращаемое значение

[ModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md)Объект класса [ModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md), хранящий координаты вектора и ссылку на эти геометрические данные профиля

Для профилей, состоящих из нескольких граней или рёбер, направление может быть не определено

#### Ссылки

[ProfileGeometryData - ](T_TFlex_Model_Model3D_Profile_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)