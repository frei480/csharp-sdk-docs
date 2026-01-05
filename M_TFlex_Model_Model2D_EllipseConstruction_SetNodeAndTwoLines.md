

Руководство по T-FLEX CAD Open API

# EllipseConstructionSetNodeAndTwoLines - метод  
  
---  
  
Эллипс проходящий через узел, касательный к двум прямым

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetNodeAndTwoLines(
	Node srcNode,
	Construction srcLine1,
	Construction srcLine2
)
```
```vb
Public Sub SetNodeAndTwoLines ( 
	srcNode As Node,
	srcLine1 As Construction,
	srcLine2 As Construction
)
```
```cpp
public:
void SetNodeAndTwoLines(
	Node^ srcNode, 
	Construction^ srcLine1, 
	Construction^ srcLine2
)
```


#### Параметры

srcNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, через который проходит эллипс
srcLine1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая прямая, которой касается эллипс
srcLine2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая прямая, которой касается эллипс

#### Ссылки

[EllipseConstruction - ](T_TFlex_Model_Model2D_EllipseConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)