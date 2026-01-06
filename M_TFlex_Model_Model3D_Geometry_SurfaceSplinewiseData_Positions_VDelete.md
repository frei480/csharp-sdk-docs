

Руководство по T-FLEX CAD Open API

# SurfaceSplinewiseDataPositionsVDelete - метод  
    
Удалить столбец. Удалить изопараметрическую кривую по V

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void VDelete(
	uint index
)
```
```vb
Public Sub VDelete ( 
	index As UInteger
)
```
```cpp
public:
void VDelete(
	unsigned int index
)
```


#### Параметры

index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер столбца

Столбцы нумеруются от нуля. Если индекс отрицательный или превышает количество столбцов, то результат не определён

#### Ссылки

[SurfaceSplinewiseDataPositions - ](T_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_Positions.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)