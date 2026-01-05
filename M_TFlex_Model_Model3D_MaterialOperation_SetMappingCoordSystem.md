

Руководство по T-FLEX CAD Open API

# MaterialOperationSetMappingCoordSystem(Int32, Point3D, Direction, Direction, Direction) - метод  
  
---  
  
Установить систему координат наложения текстуры для данной группы граней

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetMappingCoordSystem(
	int Group,
	Point3D origin,
	Direction xAxis,
	Direction yAxis,
	Direction zAxis
)
```
```vb
Public Sub SetMappingCoordSystem ( 
	Group As Integer,
	origin As Point3D,
	xAxis As Direction,
	yAxis As Direction,
	zAxis As Direction
)
```
```cpp
public:
void SetMappingCoordSystem(
	int Group, 
	Point3D^ origin, 
	Direction^ xAxis, 
	Direction^ yAxis, 
	Direction^ zAxis
)
```


#### Параметры

Group [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
origin [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    
xAxis [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
yAxis [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
zAxis [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    

Система координат определена для наложения проецированием на плоскость, цилиндр, сферу, параллелепипед. Цепочка преобразований будет состоять из трёх сдвигов и трёх поворотов.

#### Ссылки

[MaterialOperation - ](T_TFlex_Model_Model3D_MaterialOperation.md)

[SetMappingCoordSystem - перегрузка](Overload_TFlex_Model_Model3D_MaterialOperation_SetMappingCoordSystem.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)