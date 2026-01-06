

Руководство по T-FLEX CAD Open API

# RelativeNodeSetOnConstruction - метод  
    
Установка смещения относительно родительского узла по линии построения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetOnConstruction(
	Node parentNode,
	Construction srcConstruction,
	Parameter distance
)
```
```vb
Public Sub SetOnConstruction ( 
	parentNode As Node,
	srcConstruction As Construction,
	distance As Parameter
)
```
```cpp
public:
void SetOnConstruction(
	Node^ parentNode, 
	Construction^ srcConstruction, 
	Parameter^ distance
)
```


#### Параметры

parentNode [Node](T_TFlex_Model_Model2D_Node.md)
    Родительский узел
srcConstruction [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная линия построения
distance [Parameter](T_TFlex_Model_Parameter.md)
    Параметр смещения

#### Ссылки

[RelativeNode - ](T_TFlex_Model_Model2D_RelativeNode.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)