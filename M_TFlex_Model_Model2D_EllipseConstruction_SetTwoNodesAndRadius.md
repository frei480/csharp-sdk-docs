

Руководство по T-FLEX CAD Open API

# EllipseConstructionSetTwoNodesAndRadius - метод  
    
Эллипс с заданной полуосью, с заданным радиусом

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTwoNodesAndRadius(
	Node srcNode1,
	Node srcNode2,
	Parameter radius
)
```
```vb
Public Sub SetTwoNodesAndRadius ( 
	srcNode1 As Node,
	srcNode2 As Node,
	radius As Parameter
)
```
```cpp
public:
void SetTwoNodesAndRadius(
	Node^ srcNode1, 
	Node^ srcNode2, 
	Parameter^ radius
)
```


#### Параметры

srcNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел полуоси эллипса
srcNode2 [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел полуоси эллипса
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус эллипса

#### Ссылки

[EllipseConstruction - ](T_TFlex_Model_Model2D_EllipseConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)