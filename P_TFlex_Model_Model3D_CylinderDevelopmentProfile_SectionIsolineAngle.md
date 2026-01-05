

Руководство по T-FLEX CAD Open API

# CylinderDevelopmentProfileSectionIsolineAngle - свойство  
  
---  
  
Угол, определяющий изопараметрическую прямую, вдоль которой разрезается замкнутая грань

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter SectionIsolineAngle { get; set; }
```
```vb
Public Property SectionIsolineAngle As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ SectionIsolineAngle {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Линия разреза может задаваться тремя взаимоисключающими путями: 

  * кривой на грани;
  * изопараметрической прямой, проходящей через точку на поверхности;
  * углом разрезающей прямой.



#### Ссылки

[CylinderDevelopmentProfile - ](T_TFlex_Model_Model3D_CylinderDevelopmentProfile.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)