

Руководство по T-FLEX CAD Open API

# EllipseConstructionSetCenterAndLineAndRadius - метод  
  
---  
  
Эллипс проходящий через узел, касательный к прямой, с заданным радиусом

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetCenterAndLineAndRadius(
	Node centerNode,
	Construction srcLine,
	Parameter radius
)
```
```vb
Public Sub SetCenterAndLineAndRadius ( 
	centerNode As Node,
	srcLine As Construction,
	radius As Parameter
)
```
```cpp
public:
void SetCenterAndLineAndRadius(
	Node^ centerNode, 
	Construction^ srcLine, 
	Parameter^ radius
)
```


#### Параметры

centerNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, через который проходит эллипс
srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается эллипс
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус эллипса

#### Ссылки

[EllipseConstruction - ](T_TFlex_Model_Model2D_EllipseConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)