

Руководство по T-FLEX CAD Open API

# SplinewiseDataPositionsInsert - метод  
    
Вставить интерполяционную точку перед номером

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	uint Index,
	SplinewiseDataPositionsPosition point
)
```
```vb
Public Sub Insert ( 
	Index As UInteger,
	point As SplinewiseDataPositionsPosition
)
```
```cpp
public:
void Insert(
	unsigned int Index, 
	SplinewiseDataPositionsPosition^ point
)
```


#### Параметры

Index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер интерполяционной точки
point [SplinewiseDataPositionsPosition](T_TFlex_Model_Model3D_Geometry_SplinewiseData_Positions_Position.md)
    Координаты точки

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат неопределён

#### Ссылки

[SplinewiseDataPositions - ](T_TFlex_Model_Model3D_Geometry_SplinewiseData_Positions.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)