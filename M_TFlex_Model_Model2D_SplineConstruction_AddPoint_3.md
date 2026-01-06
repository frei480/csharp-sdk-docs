

Руководство по T-FLEX CAD Open API

# SplineConstructionAddPoint(Node, Boolean) - метод  
    
Добавить точку

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public int AddPoint(
	Node node,
	bool tolerant
)
```
```vb
Public Function AddPoint ( 
	node As Node,
	tolerant As Boolean
) As Integer
```
```cpp
public:
int AddPoint(
	Node^ node, 
	bool tolerant
)
```


#### Параметры

node [Node](T_TFlex_Model_Model2D_Node.md)
    Добавляемый узел
tolerant [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Является ли точка с допуском

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)Индекс узла

#### Ссылки

[SplineConstruction - ](T_TFlex_Model_Model2D_SplineConstruction.md)

[AddPoint - перегрузка](Overload_TFlex_Model_Model2D_SplineConstruction_AddPoint.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)