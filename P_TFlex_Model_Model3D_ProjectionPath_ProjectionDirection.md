

Руководство по T-FLEX CAD Open API

# ProjectionPathProjectionDirection - свойство  
    
Направление проецирования

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelDirection ProjectionDirection { get; set; }
```




#### Значение свойства

[ModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md)

Направление проецирования задаётся двумя взаимосиключающими методами: двумя точками или направлением. В настоящей версии в качестве направления можно выбирать только оси системы координат. В остальных случаях путь строится не будет. Если направление не задано, то выполняется проецирование по нормали к поверхности

#### Ссылки

[ProjectionPath - ](T_TFlex_Model_Model3D_ProjectionPath.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)