

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTangentToLineAndPolyline(Construction, Construction, Parameter, Int32) - метод  
    
Окружность, касательная к прямой и сплайну или другой полилинии

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToLineAndPolyline(
	Construction srcLine,
	Construction srcPolyline,
	Parameter radius,
	int variant
)
```
```vb
Public Sub SetTangentToLineAndPolyline ( 
	srcLine As Construction,
	srcPolyline As Construction,
	radius As Parameter,
	variant As Integer
)
```
```cpp
public:
void SetTangentToLineAndPolyline(
	Construction^ srcLine, 
	Construction^ srcPolyline, 
	Parameter^ radius, 
	int variant
)
```


#### Параметры

srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Прямая, которой касается окружность
srcPolyline [Construction](T_TFlex_Model_Model2D_Construction.md)
    Полилиния, которой касается окружность
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус окружности
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[SetTangentToLineAndPolyline - перегрузка](Overload_TFlex_Model_Model2D_CircleConstruction_SetTangentToLineAndPolyline.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)