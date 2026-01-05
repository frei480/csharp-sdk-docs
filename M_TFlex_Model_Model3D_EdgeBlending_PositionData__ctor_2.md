

Руководство по T-FLEX CAD Open API

# EdgeBlendingPositionData(Parameter, Parameter, Parameter, Parameter) - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public PositionData(
	Parameter position,
	Parameter radius1,
	Parameter radius2,
	Parameter rho
)
```
```vb
Public Sub New ( 
	position As Parameter,
	radius1 As Parameter,
	radius2 As Parameter,
	rho As Parameter
)
```
```cpp
public:
PositionData(
	Parameter^ position, 
	Parameter^ radius1, 
	Parameter^ radius2, 
	Parameter^ rho
)
```


#### Параметры

position [Parameter](T_TFlex_Model_Parameter.md)
    Позиция, задаётся в диапазоне 0..100
radius1 [Parameter](T_TFlex_Model_Parameter.md)
    1-й параметр
radius2 [Parameter](T_TFlex_Model_Parameter.md)
    2-й параметр
rho [Parameter](T_TFlex_Model_Parameter.md)
    Параметр задающий кривизну кривой: меньше 0.5 - эллипс, 0.5 - парабола, больше 0.5 - гипербола

#### Ссылки

[EdgeBlendingPositionData - ](T_TFlex_Model_Model3D_EdgeBlending_PositionData.md)

[EdgeBlendingPositionData - перегрузка](Overload_TFlex_Model_Model3D_EdgeBlending_PositionData__ctor.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)