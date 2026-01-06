

Руководство по T-FLEX CAD Open API

# SplineDataRational - свойство  
    
Установить признак рациональности сплайна

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool Rational { get; set; }
```




#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

При изменении типа на нерациональный информация о весах теряется. При изменении типа на рациональный все веса равны 1.0. Если тип не меняется, то информация о весах также не меняется

#### Ссылки

[SplineData - ](T_TFlex_Model_Model3D_Geometry_SplineData.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)