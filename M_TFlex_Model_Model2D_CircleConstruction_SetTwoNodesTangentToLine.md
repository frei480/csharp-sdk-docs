

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTwoNodesTangentToLine - метод  
  
---  
  
Окружность, проходящая через два узла, касательная к прямой

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTwoNodesTangentToLine(
	Node srcNode1,
	Node srcNode2,
	Construction srcLine,
	int variant
)
```
```vb
Public Sub SetTwoNodesTangentToLine ( 
	srcNode1 As Node,
	srcNode2 As Node,
	srcLine As Construction,
	variant As Integer
)
```
```cpp
public:
void SetTwoNodesTangentToLine(
	Node^ srcNode1, 
	Node^ srcNode2, 
	Construction^ srcLine, 
	int variant
)
```


#### Параметры

srcNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел, через который проходит окружность
srcNode2 [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел, через который проходит окружность
srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается окружность
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)