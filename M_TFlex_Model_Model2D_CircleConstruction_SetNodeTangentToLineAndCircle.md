

Руководство по T-FLEX CAD Open API

# CircleConstructionSetNodeTangentToLineAndCircle - метод  
    
Окружность, проходящая через узел, касательная к прямой и окружности

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetNodeTangentToLineAndCircle(
	Node srcNode,
	Construction srcLine,
	Construction srcCircle,
	int variant
)
```
```vb
Public Sub SetNodeTangentToLineAndCircle ( 
	srcNode As Node,
	srcLine As Construction,
	srcCircle As Construction,
	variant As Integer
)
```
```cpp
public:
void SetNodeTangentToLineAndCircle(
	Node^ srcNode, 
	Construction^ srcLine, 
	Construction^ srcCircle, 
	int variant
)
```


#### Параметры

srcNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, через который проходит окружность
srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается окружность
srcCircle [Construction](T_TFlex_Model_Model2D_Construction.md)
    Окружность, которой касается окружность
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)