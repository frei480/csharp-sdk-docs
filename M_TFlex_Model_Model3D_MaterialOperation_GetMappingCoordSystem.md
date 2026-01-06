

Руководство по T-FLEX CAD Open API

# MaterialOperationGetMappingCoordSystem - метод  
    
Получить систему координат наложения текстуры для данной группы граней

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void GetMappingCoordSystem(
	int Group,
	ref Point3D origin,
	ref Direction xAxis,
	ref Direction yAxis,
	ref Direction zAxis
)
```
```vb
Public Sub GetMappingCoordSystem ( 
	Group As Integer,
	ByRef origin As Point3D,
	ByRef xAxis As Direction,
	ByRef yAxis As Direction,
	ByRef zAxis As Direction
)
```
```cpp
public:
void GetMappingCoordSystem(
	int Group, 
	Point3D^% origin, 
	Direction^% xAxis, 
	Direction^% yAxis, 
	Direction^% zAxis
)
```


#### Параметры

Group [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
origin [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    
xAxis [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
yAxis [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
zAxis [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    

Система координат определена для наложения проецированием на плоскость, цилиндр, сферу, параллелепипед

#### Ссылки

[MaterialOperation - ](T_TFlex_Model_Model3D_MaterialOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)