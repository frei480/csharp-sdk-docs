

Руководство по T-FLEX CAD Open API

# CircleConstructionSetNodeTangentToTwoLines - метод  
  
---  
  
Окружность, проходящая через узел, касательная к двум прямым

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetNodeTangentToTwoLines(
	Node srcNode,
	Construction srcLine1,
	Construction srcLine2,
	int variant
)
```
```vb
Public Sub SetNodeTangentToTwoLines ( 
	srcNode As Node,
	srcLine1 As Construction,
	srcLine2 As Construction,
	variant As Integer
)
```
```cpp
public:
void SetNodeTangentToTwoLines(
	Node^ srcNode, 
	Construction^ srcLine1, 
	Construction^ srcLine2, 
	int variant
)
```


#### Параметры

srcNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, через который проходит окружность
srcLine1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая прямая, которой касается окружность
srcLine2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая прямая, которой касается окружность
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)