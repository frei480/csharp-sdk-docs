

Руководство по T-FLEX CAD Open API

# LineConstructionSetParallelTangentToCircle - метод  
    
Прямая, параллельная другой прямой, касательная к окружности

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetParallelTangentToCircle(
	Construction srcLine,
	Construction srcCircle,
	int variant
)
```
```vb
Public Sub SetParallelTangentToCircle ( 
	srcLine As Construction,
	srcCircle As Construction,
	variant As Integer
)
```
```cpp
public:
void SetParallelTangentToCircle(
	Construction^ srcLine, 
	Construction^ srcCircle, 
	int variant
)
```


#### Параметры

srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная прямая
srcCircle [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная окружность
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта прямой

#### Ссылки

[LineConstruction - ](T_TFlex_Model_Model2D_LineConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)