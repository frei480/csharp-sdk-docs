

Руководство по T-FLEX CAD Open API

# PipePath3DPointOnPathGetPositionOnPath - метод  
    
Возвращает позицию точки на пути по оси

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter GetPositionOnPath(
	Coordinate indCoord
)
```
```vb
Public Function GetPositionOnPath ( 
	indCoord As Coordinate
) As Parameter
```
```cpp
public:
Parameter^ GetPositionOnPath(
	Coordinate indCoord
)
```


#### Параметры

indCoord [Coordinate](T_TFlex_Model_Model3D_Coordinate.md)
    

#### Возвращаемое значение

[Parameter](T_TFlex_Model_Parameter.md)

U = X, V = Y, R = Z

#### Ссылки

[PipePath3DPointOnPath - ](T_TFlex_Model_Model3D_PipePath3D_PointOnPath.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)