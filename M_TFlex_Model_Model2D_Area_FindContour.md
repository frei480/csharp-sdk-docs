

Руководство по T-FLEX CAD Open API

# AreaFindContour(Double, Double) - метод  
  
---  
  
Автоматический поиск контуров штриховки по точке.

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool FindContour(
	double x,
	double y
)
```
```vb
Public Function FindContour ( 
	x As Double,
	y As Double
) As Boolean
```
```cpp
public:
bool FindContour(
	double x, 
	double y
)
```


#### Параметры

x [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата X точки поиска
y [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата Y точки поиска

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)true, если найден хотя бы один контур

Последовательность вызовов данной функции должна завершаться вызовом функции ApplyContours

#### Ссылки

[Area - ](T_TFlex_Model_Model2D_Area.md)

[FindContour - перегрузка](Overload_TFlex_Model_Model2D_Area_FindContour.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)