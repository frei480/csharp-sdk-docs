

Руководство по T-FLEX CAD Open API

# CylinderDevelopmentProfileSectionCurve - свойство  
    
Кривая, вдоль которой разрезается замкнутая грань

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelWire SectionCurve { get; set; }
```




#### Значение свойства

[ModelWire](T_TFlex_Model_Model3D_Geometry_ModelWire.md)

В настоящей версии в качестве кривой можно выбирать только ребро. В остальных случаях профиль строится не будет. Линия разреза может задаваться тремя взаимоисключающими путями: 

  * кривой на грани;
  * изопараметрической прямой, проходящей через точку на поверхности;
  * углом разрезающей прямой.



#### Ссылки

[CylinderDevelopmentProfile - ](T_TFlex_Model_Model3D_CylinderDevelopmentProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)