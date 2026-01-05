

Руководство по T-FLEX CAD Open API

# CircleConstructionSetCenterAndLine - метод  
  
---  
  
Окружность с центром в узле, касательная к прямой

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetCenterAndLine(
	Node centerNode,
	Construction srcLine
)
```
```vb
Public Sub SetCenterAndLine ( 
	centerNode As Node,
	srcLine As Construction
)
```
```cpp
public:
void SetCenterAndLine(
	Node^ centerNode, 
	Construction^ srcLine
)
```


#### Параметры

centerNode [Node](T_TFlex_Model_Model2D_Node.md)
    Центр окружности
srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается окружность

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)