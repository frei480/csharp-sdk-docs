

Руководство по T-FLEX CAD Open API

# OperationGeometryDataDirection - свойство  
    
Получить направление

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelDirection Direction { get; }
```




#### Значение свойства

[ModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md)

| Возвращаемое направление зависит от типа операции. Операция | Направление |
| --- | --- |
| Выталкивание | Направление выталкивания |
| Вращение | Ось вращения |
| Линейный массив | Направление копирования |
| Круговой массив | Ось вращения |
| Спираль | Ось спирали |
| Пружина | Ось пружины |
| Уклон | Направление уклона |
  
#### Ссылки

[OperationGeometryData - ](T_TFlex_Model_Model3D_Operation_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)