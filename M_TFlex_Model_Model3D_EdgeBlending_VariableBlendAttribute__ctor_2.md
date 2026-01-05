

Руководство по T-FLEX CAD Open API

# EdgeBlendingVariableBlendAttribute(Parameter, Parameter, Parameter) - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public VariableBlendAttribute(
	Parameter radius1,
	Parameter radius2,
	Parameter rho
)
```
```vb
Public Sub New ( 
	radius1 As Parameter,
	radius2 As Parameter,
	rho As Parameter
)
```
```cpp
public:
VariableBlendAttribute(
	Parameter^ radius1, 
	Parameter^ radius2, 
	Parameter^ rho
)
```


#### Параметры

radius1 [Parameter](T_TFlex_Model_Parameter.md)
    1-й параметр
radius2 [Parameter](T_TFlex_Model_Parameter.md)
    2-й параметр
rho [Parameter](T_TFlex_Model_Parameter.md)
    Параметр задающий кривизну: меньше 0.5 - эллипс, 0.5 - парабола, больше 0.5 - гипербола

#### Ссылки

[EdgeBlendingVariableBlendAttribute - ](T_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute.md)

[EdgeBlendingVariableBlendAttribute - перегрузка](Overload_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute__ctor.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)