

Руководство по T-FLEX CAD Open API

# LinearDimensionSetArcLength - метод  
    
Установка параметров размера - длины дуги

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetArcLength(
	Object2D arcOrCircle,
	Node node1,
	Node node2,
	bool linesAreRadial
)
```
```vb
Public Sub SetArcLength ( 
	arcOrCircle As Object2D,
	node1 As Node,
	node2 As Node,
	linesAreRadial As Boolean
)
```
```cpp
public:
void SetArcLength(
	Object2D^ arcOrCircle, 
	Node^ node1, 
	Node^ node2, 
	bool linesAreRadial
)
```


#### Параметры

arcOrCircle [Object2D](T_TFlex_Model_Model2D_Object2D.md)
    Измеряемая дуга, либо окружность, часть которой меряется
node1 [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, с которого (против часовой стрелки) начинается измерение
node2 [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, на котором (против часовой стрелки) заканчивается измерение
linesAreRadial [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает на то, что выносныме линии размера должны быть радиальными (иначе - параллельны друг другу)

#### Ссылки

[LinearDimension - ](T_TFlex_Model_Model2D_LinearDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)