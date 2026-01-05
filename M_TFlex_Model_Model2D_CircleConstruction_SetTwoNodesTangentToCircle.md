

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTwoNodesTangentToCircle - метод  
  
---  
  
Окружность, проходящая через два узла, касательная к окружности

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTwoNodesTangentToCircle(
	Node srcNode1,
	Node srcNode2,
	Construction srcCircle,
	int variant
)
```
```vb
Public Sub SetTwoNodesTangentToCircle ( 
	srcNode1 As Node,
	srcNode2 As Node,
	srcCircle As Construction,
	variant As Integer
)
```
```cpp
public:
void SetTwoNodesTangentToCircle(
	Node^ srcNode1, 
	Node^ srcNode2, 
	Construction^ srcCircle, 
	int variant
)
```


#### Параметры

srcNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел, через который проходит окружность
srcNode2 [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел, через который проходит окружность
srcCircle [Construction](T_TFlex_Model_Model2D_Construction.md)
    Окружность, которой касается окружность
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)