

Руководство по T-FLEX CAD Open API

# OutlineEvaluatePoint - метод  
    
Получить точку на кривой по параметру iU 

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool EvaluatePoint(
	double iU,
	ref Point oPoint
)
```
```vb
Public Function EvaluatePoint ( 
	iU As Double,
	ByRef oPoint As Point
) As Boolean
```
```cpp
public:
bool EvaluatePoint(
	double iU, 
	Point% oPoint
)
```


#### Параметры

iU [Double](https://learn.microsoft.com/dotnet/api/system.double)
     Параметр на кривой, в котором вычисляется точка 
oPoint [Point](T_TFlex_Drawing_Point.md)
     Вычисленная точка 

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean) true - в случае успеха 

#### Ссылки

[Outline - ](T_TFlex_Model_Model2D_Outline.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)