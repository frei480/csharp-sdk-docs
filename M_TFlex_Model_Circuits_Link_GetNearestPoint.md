

Руководство по T-FLEX CAD Open API

# LinkGetNearestPoint - метод  
  **Пространство имён:** [TFlex.Model.Circuits](N_TFlex_Model_Circuits.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Point GetNearestPoint(
	Point position,
	double maxDistance,
	int minNeighbours
)
```
```vb
Public Function GetNearestPoint ( 
	position As Point,
	maxDistance As Double,
	minNeighbours As Integer
) As Point
```
```cpp
public:
Point^ GetNearestPoint(
	Point position, 
	double maxDistance, 
	int minNeighbours
)
```


#### Параметры

position [Point](T_TFlex_Drawing_Point.md)
    
maxDistance [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
minNeighbours [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    

#### Возвращаемое значение

[Point](T_TFlex_Model_Circuits_Graph_Point.md)

#### Ссылки

[Link - ](T_TFlex_Model_Circuits_Link.md)

[TFlex.Model.Circuits - пространство имён](N_TFlex_Model_Circuits.md)