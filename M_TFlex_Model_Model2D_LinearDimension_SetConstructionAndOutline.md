

Руководство по T-FLEX CAD Open API

# LinearDimensionSetConstructionAndOutline - метод  
  
---  
  
Установка параметров размера между линией построения и линией изображения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetConstructionAndOutline(
	Construction line1,
	Node node1,
	Outline line2,
	bool isOnEnd2
)
```
```vb
Public Sub SetConstructionAndOutline ( 
	line1 As Construction,
	node1 As Node,
	line2 As Outline,
	isOnEnd2 As Boolean
)
```
```cpp
public:
void SetConstructionAndOutline(
	Construction^ line1, 
	Node^ node1, 
	Outline^ line2, 
	bool isOnEnd2
)
```


#### Параметры

line1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая
node1 [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, задающий положение начала выносной линии на прямой
line2 [Outline](T_TFlex_Model_Model2D_Outline.md)
    Отрезок
isOnEnd2 [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает на то, что размер прикреплен к концу отрезка (иначе - к началу)

#### Ссылки

[LinearDimension - ](T_TFlex_Model_Model2D_LinearDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)