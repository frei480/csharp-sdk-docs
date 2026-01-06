

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTangentToTwoLines(Construction, Construction, Parameter, Int32) - метод  
    
Окружность, касательная к двум прямым

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToTwoLines(
	Construction srcLine1,
	Construction srcLine2,
	Parameter radius,
	int variant
)
```
```vb
Public Sub SetTangentToTwoLines ( 
	srcLine1 As Construction,
	srcLine2 As Construction,
	radius As Parameter,
	variant As Integer
)
```
```cpp
public:
void SetTangentToTwoLines(
	Construction^ srcLine1, 
	Construction^ srcLine2, 
	Parameter^ radius, 
	int variant
)
```


#### Параметры

srcLine1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая прямая, которой касается окружность
srcLine2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая прямая, которой касается окружность
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус окружности
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[SetTangentToTwoLines - перегрузка](Overload_TFlex_Model_Model2D_CircleConstruction_SetTangentToTwoLines.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)