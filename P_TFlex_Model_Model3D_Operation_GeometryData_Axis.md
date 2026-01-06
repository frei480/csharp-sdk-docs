

Руководство по T-FLEX CAD Open API

# OperationGeometryDataAxis - свойство  
    
Получить ось

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelAxis Axis { get; }
```
```vb
Public ReadOnly Property Axis As ModelAxis
	Get
```
```cpp
public:
property ModelAxis^ Axis {
	ModelAxis^ get ();
}
```


#### Значение свойства

[ModelAxis](T_TFlex_Model_Model3D_Geometry_ModelAxis.md)

| Возвращаемая ось зависит от типа операции. Операция | Ось |
| --- | --- |
| Вращение | Ось вращения |
| Круговой массив | Ось вращения |
| Спираль | Ось спирали |
| Пружина | Ось пружины |
  
#### Ссылки

[OperationGeometryData - ](T_TFlex_Model_Model3D_Operation_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)