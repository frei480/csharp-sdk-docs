

Руководство по T-FLEX CAD Open API

# EllipseConstructionSetTwoNodesAndLine - метод  
    
Эллипс с заданной полуосью, касательный к прямой

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTwoNodesAndLine(
	Node srcNode1,
	Node srcNode2,
	Construction srcLine
)
```
```vb
Public Sub SetTwoNodesAndLine ( 
	srcNode1 As Node,
	srcNode2 As Node,
	srcLine As Construction
)
```
```cpp
public:
void SetTwoNodesAndLine(
	Node^ srcNode1, 
	Node^ srcNode2, 
	Construction^ srcLine
)
```


#### Параметры

srcNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел полуоси эллипса
srcNode2 [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел полуоси эллипса
srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается эллипс

#### Ссылки

[EllipseConstruction - ](T_TFlex_Model_Model2D_EllipseConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)