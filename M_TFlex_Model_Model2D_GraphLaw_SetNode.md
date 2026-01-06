

Руководство по T-FLEX CAD Open API

# GraphLawSetNode - метод  
    
Установка узла по номеру

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool SetNode(
	uint index,
	Point value
)
```
```vb
Public Function SetNode ( 
	index As UInteger,
	value As Point
) As Boolean
```
```cpp
public:
bool SetNode(
	unsigned int index, 
	Point value
)
```


#### Параметры

index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    
value [Point](T_TFlex_Drawing_Point.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Узел изменяется только в том случае, если заданное значение аргумента соответствует порядку значений аргументов остальных узлов (по возрастанию)

#### Ссылки

[GraphLaw - ](T_TFlex_Model_Model2D_GraphLaw.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)