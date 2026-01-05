

Руководство по T-FLEX CAD Open API

# ParametricQuantity - свойство  
  
---  
  
Количество копий

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter Quantity { get; set; }
```
```vb
Public Property Quantity As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ Quantity {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Количество копий должно быть больше одного. Количество копий округляется до ближайшего целого, меньшего заданного

#### Ссылки

[Parametric - ](T_TFlex_Model_Model3D_Parametric.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)