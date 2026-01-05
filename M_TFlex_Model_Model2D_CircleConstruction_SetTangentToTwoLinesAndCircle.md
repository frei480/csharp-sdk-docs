

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTangentToTwoLinesAndCircle - метод  
  
---  
  
Окружность, касательная к двум прямым и окружности

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToTwoLinesAndCircle(
	Construction srcLine1,
	Construction srcLine2,
	Construction srcCircle,
	int variant
)
```
```vb
Public Sub SetTangentToTwoLinesAndCircle ( 
	srcLine1 As Construction,
	srcLine2 As Construction,
	srcCircle As Construction,
	variant As Integer
)
```
```cpp
public:
void SetTangentToTwoLinesAndCircle(
	Construction^ srcLine1, 
	Construction^ srcLine2, 
	Construction^ srcCircle, 
	int variant
)
```


#### Параметры

srcLine1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая прямая, которой касается окружность
srcLine2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая прямая, которой касается окружность
srcCircle [Construction](T_TFlex_Model_Model2D_Construction.md)
    Окружность, которой касается окружность
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)