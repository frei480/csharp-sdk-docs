

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTangentToCircleAndLine - метод  
    
Окружность, касательная к окружности и прямой

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToCircleAndLine(
	Construction srcCircle,
	Construction srcLine,
	Parameter radius,
	int variant
)
```
```vb
Public Sub SetTangentToCircleAndLine ( 
	srcCircle As Construction,
	srcLine As Construction,
	radius As Parameter,
	variant As Integer
)
```
```cpp
public:
void SetTangentToCircleAndLine(
	Construction^ srcCircle, 
	Construction^ srcLine, 
	Parameter^ radius, 
	int variant
)
```


#### Параметры

srcCircle [Construction](T_TFlex_Model_Model2D_Construction.md)
    Окружность, которой касается окружность
srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается окружность
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус окружности
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)