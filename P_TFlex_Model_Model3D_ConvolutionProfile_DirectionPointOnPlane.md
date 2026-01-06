

Руководство по T-FLEX CAD Open API

# ConvolutionProfileDirectionPointOnPlane - свойство  
    
Вторая точка в плоскости сворачиваемго контура

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D DirectionPointOnPlane { get; set; }
```




#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Эта точка и вторая точка на поверхности задают направление свертки. В настоящей версии в качестве точки можно выбирать только 3D узлы. В остальных случаях профиль строится не будет

#### Ссылки

[ConvolutionProfile - ](T_TFlex_Model_Model3D_ConvolutionProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)