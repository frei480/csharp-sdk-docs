

Руководство по T-FLEX CAD Open API

# OperationGeometryDataCurve - свойство  
  
---  
  
Получить кривую, на которой лежит граница листовой операции

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelCurve Curve { get; }
```
```vb
Public ReadOnly Property Curve As ModelCurve
	Get
```
```cpp
public:
property ModelCurve^ Curve {
	ModelCurve^ get ();
}
```


#### Значение свойства

[ModelCurve](T_TFlex_Model_Model3D_Geometry_ModelCurve.md)

Для операций, состоящих из нескольких рёбер, кривая может быть не определена

#### Ссылки

[OperationGeometryData - ](T_TFlex_Model_Model3D_Operation_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)