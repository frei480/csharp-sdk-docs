

Руководство по T-FLEX CAD Open API

# SurfaceSplineDataControlNetVInsert - метод  
  
---  
  
Вставить столбец. Вставить изопараметрическую кривую по V

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void VInsert(
	uint Index
)
```
```vb
Public Sub VInsert ( 
	Index As UInteger
)
```
```cpp
public:
void VInsert(
	unsigned int Index
)
```


#### Параметры

Index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер столбца

Столбцы нумеруются от нуля. Если индекс отрицательный или превышает количество столбцов, то результат неопределён

#### Ссылки

[SurfaceSplineDataControlNet - ](T_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)