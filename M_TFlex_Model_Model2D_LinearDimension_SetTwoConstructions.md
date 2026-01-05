

Руководство по T-FLEX CAD Open API

# LinearDimensionSetTwoConstructions - метод  
  
---  
  
Установка параметров размера между двумя линиями построения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTwoConstructions(
	Construction line1,
	Node node1,
	Construction line2,
	Node node2
)
```
```vb
Public Sub SetTwoConstructions ( 
	line1 As Construction,
	node1 As Node,
	line2 As Construction,
	node2 As Node
)
```
```cpp
public:
void SetTwoConstructions(
	Construction^ line1, 
	Node^ node1, 
	Construction^ line2, 
	Node^ node2
)
```


#### Параметры

line1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая прямая
node1 [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, задающий положение начала выносной линии на прямой
line2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая прямая
node2 [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, задающий положение начала выносной линии на прямой

#### Ссылки

[LinearDimension - ](T_TFlex_Model_Model2D_LinearDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)