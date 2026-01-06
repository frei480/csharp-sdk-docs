

Руководство по T-FLEX CAD Open API

# SurfaceSplineDataControlNetUDelete - метод  
    
Удалить строку. Удалить изопараметрическую кривую по U

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void UDelete(
	uint index
)
```
```vb
Public Sub UDelete ( 
	index As UInteger
)
```
```cpp
public:
void UDelete(
	unsigned int index
)
```


#### Параметры

index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер строки

Строки нумеруются от нуля. Если индекс отрицательный или превышает количество строк, то результат не определён

#### Ссылки

[SurfaceSplineDataControlNet - ](T_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)