

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTwoNodes - метод  
  
---  
  
Окружность, проходящая через два узла

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTwoNodes(
	Node srcNode1,
	Node srcNode2,
	Parameter radius,
	int variant
)
```
```vb
Public Sub SetTwoNodes ( 
	srcNode1 As Node,
	srcNode2 As Node,
	radius As Parameter,
	variant As Integer
)
```
```cpp
public:
void SetTwoNodes(
	Node^ srcNode1, 
	Node^ srcNode2, 
	Parameter^ radius, 
	int variant
)
```


#### Параметры

srcNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел, через который проходит окружность
srcNode2 [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел, через который проходит окружность
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус окружности
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)