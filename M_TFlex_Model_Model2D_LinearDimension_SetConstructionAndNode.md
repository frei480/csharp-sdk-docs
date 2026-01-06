

Руководство по T-FLEX CAD Open API

# LinearDimensionSetConstructionAndNode - метод  
    
Установка параметров размера между линией построения и узлом

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetConstructionAndNode(
	Construction line1,
	Node node1,
	Node node2
)
```
```vb
Public Sub SetConstructionAndNode ( 
	line1 As Construction,
	node1 As Node,
	node2 As Node
)
```
```cpp
public:
void SetConstructionAndNode(
	Construction^ line1, 
	Node^ node1, 
	Node^ node2
)
```


#### Параметры

line1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая
node1 [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, задающий положение начала выносной линии на прямой
node2 [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, до которого измеряется расстояние

#### Ссылки

[LinearDimension - ](T_TFlex_Model_Model2D_LinearDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)