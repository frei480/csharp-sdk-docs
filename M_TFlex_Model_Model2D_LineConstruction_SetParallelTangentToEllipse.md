

Руководство по T-FLEX CAD Open API

# LineConstructionSetParallelTangentToEllipse - метод  
    
Прямая, параллельная другой прямой, касательная к эллипсу

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetParallelTangentToEllipse(
	Construction srcLine,
	Construction srcEllipse,
	int variant
)
```
```vb
Public Sub SetParallelTangentToEllipse ( 
	srcLine As Construction,
	srcEllipse As Construction,
	variant As Integer
)
```
```cpp
public:
void SetParallelTangentToEllipse(
	Construction^ srcLine, 
	Construction^ srcEllipse, 
	int variant
)
```


#### Параметры

srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходный узел
srcEllipse [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходный эллипс
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта прямой

#### Ссылки

[LineConstruction - ](T_TFlex_Model_Model2D_LineConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)