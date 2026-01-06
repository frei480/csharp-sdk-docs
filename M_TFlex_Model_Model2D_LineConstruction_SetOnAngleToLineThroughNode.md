

Руководство по T-FLEX CAD Open API

# LineConstructionSetOnAngleToLineThroughNode - метод  
    
Прямая, проходящая через узел, под углом к другой прямой

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetOnAngleToLineThroughNode(
	Construction srcLine,
	Node srcNode,
	Parameter angle
)
```
```vb
Public Sub SetOnAngleToLineThroughNode ( 
	srcLine As Construction,
	srcNode As Node,
	angle As Parameter
)
```
```cpp
public:
void SetOnAngleToLineThroughNode(
	Construction^ srcLine, 
	Node^ srcNode, 
	Parameter^ angle
)
```


#### Параметры

srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная линия построения (прямая)
srcNode [Node](T_TFlex_Model_Model2D_Node.md)
    Исходный узел
angle [Parameter](T_TFlex_Model_Parameter.md)
    Устанавливаемое значение угла в градусах

#### Ссылки

[LineConstruction - ](T_TFlex_Model_Model2D_LineConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)