

Руководство по T-FLEX CAD Open API

# CircleConstructionSetNodeTangentToTwoCircles - метод  
  
---  
  
Окружность, проходящая через узел, касательная к двум окружностям

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetNodeTangentToTwoCircles(
	Node srcNode,
	Construction srcCircle1,
	Construction srcCircle2,
	int variant
)
```
```vb
Public Sub SetNodeTangentToTwoCircles ( 
	srcNode As Node,
	srcCircle1 As Construction,
	srcCircle2 As Construction,
	variant As Integer
)
```
```cpp
public:
void SetNodeTangentToTwoCircles(
	Node^ srcNode, 
	Construction^ srcCircle1, 
	Construction^ srcCircle2, 
	int variant
)
```


#### Параметры

srcNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, через который проходит окружность
srcCircle1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая окружность, которой касается окружность
srcCircle2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая окружность, которой касается окружность
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)