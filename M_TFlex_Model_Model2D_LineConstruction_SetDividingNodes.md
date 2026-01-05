

Руководство по T-FLEX CAD Open API

# LineConstructionSetDividingNodes - метод  
  
---  
  
Прямая, перпендикулярная отрезку между двумя узлами, делящая отрезок в заданной пропорции

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetDividingNodes(
	Node srcNode1,
	Node srcNode2,
	Parameter param
)
```
```vb
Public Sub SetDividingNodes ( 
	srcNode1 As Node,
	srcNode2 As Node,
	param As Parameter
)
```
```cpp
public:
void SetDividingNodes(
	Node^ srcNode1, 
	Node^ srcNode2, 
	Parameter^ param
)
```


#### Параметры

srcNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый исходный узел
srcNode2 [Node](T_TFlex_Model_Model2D_Node.md)
    Второй исходный узел
param [Parameter](T_TFlex_Model_Parameter.md)
    Значение параметра, коэффициент. Имеет значение 0, если результирующая прямая продит через первый узел, 1, если проходит черз второй узел, 0.5, если делит отрезок пополам. Может принимать любое значение

#### Ссылки

[LineConstruction - ](T_TFlex_Model_Model2D_LineConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)