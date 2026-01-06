

Руководство по T-FLEX CAD Open API

# PiecewiseDataSegmentsSetDelete - метод  
    
Удалить сегмент по номеру

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Delete(
	uint index
)
```




#### Параметры

index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер сегмента

Сегменты нумеруются от нуля. Если индекс отрицательный или превышает количество сегментов, то результат неопределён

#### Ссылки

[PiecewiseDataSegmentsSet - ](T_TFlex_Model_Model3D_Geometry_PiecewiseData_SegmentsSet.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)