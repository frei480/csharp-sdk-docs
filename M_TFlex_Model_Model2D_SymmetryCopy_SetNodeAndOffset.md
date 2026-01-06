

Руководство по T-FLEX CAD Open API

# SymmetryCopySetNodeAndOffset - метод  
    
Установка оси симметрии по узлу и смещению

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetNodeAndOffset(
	Node baseNode,
	double baseX,
	double baseY,
	double dX,
	double dY
)
```
```vb
Public Sub SetNodeAndOffset ( 
	baseNode As Node,
	baseX As Double,
	baseY As Double,
	dX As Double,
	dY As Double
)
```
```cpp
public:
void SetNodeAndOffset(
	Node^ baseNode, 
	double baseX, 
	double baseY, 
	double dX, 
	double dY
)
```


#### Параметры

baseNode [Node](T_TFlex_Model_Model2D_Node.md)
    Базовый узел - первая точка, определяющая ось
baseX [Double](https://learn.microsoft.com/dotnet/api/system.double)
    X-координата базовой точки
baseY [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Y-координата базовой точки
dX [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение по оси X для второй точки, определяющей ось
dY [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение по оси Y для второй точки, определяющей ось

Если базовый узел не задан (NULL), то привязка происходит по точке с заданными координатами. В противном случае - координаты игнорируются

#### Ссылки

[SymmetryCopy - ](T_TFlex_Model_Model2D_SymmetryCopy.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)