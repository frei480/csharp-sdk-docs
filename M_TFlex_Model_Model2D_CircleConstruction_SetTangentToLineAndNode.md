

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTangentToLineAndNode - метод  
    
Окружность, касательная к прямой, проходящая через узел

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToLineAndNode(
	Construction srcLine,
	Node srcNode,
	Parameter radius,
	int variant
)
```
```vb
Public Sub SetTangentToLineAndNode ( 
	srcLine As Construction,
	srcNode As Node,
	radius As Parameter,
	variant As Integer
)
```
```cpp
public:
void SetTangentToLineAndNode(
	Construction^ srcLine, 
	Node^ srcNode, 
	Parameter^ radius, 
	int variant
)
```


#### Параметры

srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается окружность
srcNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, через который проходит окружность
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус окружности
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)