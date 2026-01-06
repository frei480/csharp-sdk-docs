

Руководство по T-FLEX CAD Open API

# BodyNormalizeIfPlanarClosedWire - метод  
    
Если тело является плоским замкнутым контуром, то обход по нему можно ориентировать против часовой стрелки согласно нормали к этой плоскости

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool NormalizeIfPlanarClosedWire(
	BaseDirection direction
)
```
```vb
Public Function NormalizeIfPlanarClosedWire ( 
	direction As BaseDirection
) As Boolean
```
```cpp
public:
bool NormalizeIfPlanarClosedWire(
	BaseDirection^ direction
)
```


#### Параметры

direction [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Нормаль к плоскости заданного контура

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[Body - ](T_TFlex_Model_Model3D_Geometry_Body.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)