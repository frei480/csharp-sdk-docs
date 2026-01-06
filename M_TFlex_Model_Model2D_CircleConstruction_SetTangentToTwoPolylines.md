

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTangentToTwoPolylines - метод  
    
Окружность, касательная к двум сплайнам или другим полилиниям

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToTwoPolylines(
	Construction srcPolyline1,
	Construction srcPolyline2,
	Parameter radius,
	int variant
)
```
```vb
Public Sub SetTangentToTwoPolylines ( 
	srcPolyline1 As Construction,
	srcPolyline2 As Construction,
	radius As Parameter,
	variant As Integer
)
```
```cpp
public:
void SetTangentToTwoPolylines(
	Construction^ srcPolyline1, 
	Construction^ srcPolyline2, 
	Parameter^ radius, 
	int variant
)
```


#### Параметры

srcPolyline1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая полилиния, которой касается окружность
srcPolyline2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая полилиния, которой касается окружность
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус окружности
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)