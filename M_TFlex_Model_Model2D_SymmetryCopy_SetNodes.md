

Руководство по T-FLEX CAD Open API

# SymmetryCopySetNodes - метод  
    
Установка оси симметрии по двум узлам

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetNodes(
	Node firstNode,
	double firstX,
	double firstY,
	Node secondNode,
	double secondX,
	double secondY
)
```
```vb
Public Sub SetNodes ( 
	firstNode As Node,
	firstX As Double,
	firstY As Double,
	secondNode As Node,
	secondX As Double,
	secondY As Double
)
```
```cpp
public:
void SetNodes(
	Node^ firstNode, 
	double firstX, 
	double firstY, 
	Node^ secondNode, 
	double secondX, 
	double secondY
)
```


#### Параметры

firstNode [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел, определяющий ось
firstX [Double](https://learn.microsoft.com/dotnet/api/system.double)
    X-координата первой точи, определяющей ось
firstY [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Y-координата первой точи, определяющей ось
secondNode [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел, определяющий ось
secondX [Double](https://learn.microsoft.com/dotnet/api/system.double)
    X-координата второй точи, определяющей ось
secondY [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Y-координата второй точи, определяющей ось

Если какой-либо из узлов не задан (NULL), то привязка происходит по точке с заданными координатами. В противном случае - координаты игнорируются

#### Ссылки

[SymmetryCopy - ](T_TFlex_Model_Model2D_SymmetryCopy.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)