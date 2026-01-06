

Руководство по T-FLEX CAD Open API

# ConstructionDimensionSetConstruction - метод  
    
Прикрепление размера к линии построения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetConstruction(
	Construction horizontalLine,
	Node node
)
```
```vb
Public Sub SetConstruction ( 
	horizontalLine As Construction,
	node As Node
)
```
```cpp
public:
void SetConstruction(
	Construction^ horizontalLine, 
	Node^ node
)
```


#### Параметры

horizontalLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Линия построения, к которой прикрепляется размер
node [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, до которого рисуется выносная линия размера

#### Ссылки

[ConstructionDimension - ](T_TFlex_Model_Model2D_ConstructionDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)