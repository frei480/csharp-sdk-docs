

Руководство по T-FLEX CAD Open API

# EllipseConstructionSetCenterAndLineAndNode - метод  
  
---  
  
Эллипс с центром в узле, касательный к прямой, проходящий через узел

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetCenterAndLineAndNode(
	Node centerNode,
	Construction srcLine,
	Node srcNode
)
```
```vb
Public Sub SetCenterAndLineAndNode ( 
	centerNode As Node,
	srcLine As Construction,
	srcNode As Node
)
```
```cpp
public:
void SetCenterAndLineAndNode(
	Node^ centerNode, 
	Construction^ srcLine, 
	Node^ srcNode
)
```


#### Параметры

centerNode [Node](T_TFlex_Model_Model2D_Node.md)
    Центр эллипса
srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается эллипс
srcNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, через который проходит эллипс

#### Ссылки

[EllipseConstruction - ](T_TFlex_Model_Model2D_EllipseConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)