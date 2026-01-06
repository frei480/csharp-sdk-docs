

Руководство по T-FLEX CAD Open API

# FormlimitsSetConstruction - метод  
    
Установка параметров привязки к прямой

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetConstruction(
	Construction line,
	Node node,
	Parameter offset
)
```
```vb
Public Sub SetConstruction ( 
	line As Construction,
	node As Node,
	offset As Parameter
)
```
```cpp
public:
void SetConstruction(
	Construction^ line, 
	Node^ node, 
	Parameter^ offset
)
```


#### Параметры

line [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая
node [Node](T_TFlex_Model_Model2D_Node.md)
    Узел на прямой
offset [Parameter](T_TFlex_Model_Parameter.md)
    Смещение точки привязки по прямой относительно узла

#### Ссылки

[Formlimits - ](T_TFlex_Model_Model2D_Formlimits.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)