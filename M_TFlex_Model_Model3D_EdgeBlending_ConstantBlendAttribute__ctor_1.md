

Руководство по T-FLEX CAD Open API

# EdgeBlendingConstantBlendAttribute(Parameter, Parameter, Parameter) - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ConstantBlendAttribute(
	Parameter radius,
	Parameter setbackStart,
	Parameter setbackEnd
)
```
```vb
Public Sub New ( 
	radius As Parameter,
	setbackStart As Parameter,
	setbackEnd As Parameter
)
```
```cpp
public:
ConstantBlendAttribute(
	Parameter^ radius, 
	Parameter^ setbackStart, 
	Parameter^ setbackEnd
)
```


#### Параметры

radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус скругления
setbackStart [Parameter](T_TFlex_Model_Parameter.md)
    Параметр используемый для задания чемоданного угла от начала ребра, может быть равен 0
setbackEnd [Parameter](T_TFlex_Model_Parameter.md)
    Параметр используемый для задания чемоданного угла от конца ребра, может быть равен 0

#### Ссылки

[EdgeBlendingConstantBlendAttribute - ](T_TFlex_Model_Model3D_EdgeBlending_ConstantBlendAttribute.md)

[EdgeBlendingConstantBlendAttribute - перегрузка](Overload_TFlex_Model_Model3D_EdgeBlending_ConstantBlendAttribute__ctor.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)