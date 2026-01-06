

Руководство по T-FLEX CAD Open API

# RoughnessSymbolSetNode - метод  
    
Установка параметров привязки к узлу

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetNode(
	Node nod,
	Parameter dX,
	Parameter dY
)
```
```vb
Public Sub SetNode ( 
	nod As Node,
	dX As Parameter,
	dY As Parameter
)
```
```cpp
public:
void SetNode(
	Node^ nod, 
	Parameter^ dX, 
	Parameter^ dY
)
```


#### Параметры

nod [Node](T_TFlex_Model_Model2D_Node.md)
    Узел привязки
dX [Parameter](T_TFlex_Model_Parameter.md)
    Смещение относительно узла привязки по оси X
dY [Parameter](T_TFlex_Model_Parameter.md)
    Смещение относительно узла привязки по оси Y

#### Ссылки

[RoughnessSymbol - ](T_TFlex_Model_Model2D_RoughnessSymbol.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)