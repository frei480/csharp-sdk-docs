

Руководство по T-FLEX CAD Open API

# ProfileGeometryDataCurveAxis - свойство  
  
---  
  
Если профиль лежит на окружности или эллипсе, то можно получить их ось

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelAxis CurveAxis { get; }
```
```vb
Public ReadOnly Property CurveAxis As ModelAxis
	Get
```
```cpp
public:
property ModelAxis^ CurveAxis {
	ModelAxis^ get ();
}
```


#### Возвращаемое значение

[ModelAxis](T_TFlex_Model_Model3D_Geometry_ModelAxis.md)Объект класса [ModelAxis](T_TFlex_Model_Model3D_Geometry_ModelAxis.md), хранящий координаты оси и ссылку на эти геометрические данные профиля

Для профилей, состоящих из нескольких граней или рёбер, ось может быть не определена

#### Ссылки

[ProfileGeometryData - ](T_TFlex_Model_Model3D_Profile_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)