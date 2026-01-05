

Руководство по T-FLEX CAD Open API

# OnAxisWorkplaneAngle - свойство  
  
---  
  
Угол поворота

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter Angle { get; set; }
```
```vb
Public Property Angle As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ Angle {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Доворот рабочей плоскости задаётся тремя взаимоисключающими способами : \- точкой, через которую проходит рабочая плоскость; \- параметром угла поворота; \- поверхностью, которой касается рабочая плоскость.

#### Ссылки

[OnAxisWorkplane - ](T_TFlex_Model_Model3D_OnAxisWorkplane.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)