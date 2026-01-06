

Руководство по T-FLEX CAD Open API

# LeaderNoteSetArrowConstructionLine - метод  
    
Установка параметров привязки стрелки к прямой

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetArrowConstructionLine(
	Construction line,
	Node nod,
	Parameter offset
)
```
```vb
Public Sub SetArrowConstructionLine ( 
	line As Construction,
	nod As Node,
	offset As Parameter
)
```
```cpp
public:
void SetArrowConstructionLine(
	Construction^ line, 
	Node^ nod, 
	Parameter^ offset
)
```


#### Параметры

line [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая привязки
nod [Node](T_TFlex_Model_Model2D_Node.md)
    Узел привязки (на прямой)
offset [Parameter](T_TFlex_Model_Parameter.md)
    Смещение точки привязки по прямой относительно узла

#### Ссылки

[LeaderNote - ](T_TFlex_Model_Model2D_LeaderNote.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)