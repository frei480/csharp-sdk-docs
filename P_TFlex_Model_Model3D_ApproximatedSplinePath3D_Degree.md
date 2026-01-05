

Руководство по T-FLEX CAD Open API

# ApproximatedSplinePath3DDegree - свойство  
  
---  
  
Степень сплайна

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter Degree { get; set; }
```
```vb
Public Property Degree As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ Degree {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Значение степени округляется до ближайшего целого. Степень должна быть больше нуля и меньше числа точек.

#### Ссылки

[ApproximatedSplinePath3D - ](T_TFlex_Model_Model3D_ApproximatedSplinePath3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)