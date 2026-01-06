

Руководство по T-FLEX CAD Open API

# SurfacePiecewiseDataSegmentsSetUInsert - метод  
    
Вставить строку. Вставить сегменты по U

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void UInsert(
	uint Index
)
```
```vb
Public Sub UInsert ( 
	Index As UInteger
)
```
```cpp
public:
void UInsert(
	unsigned int Index
)
```


#### Параметры

Index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер строки

Строки нумеруются от нуля. Если индекс отрицательный или превышает количество строк, то результат не определён

#### Ссылки

[SurfacePiecewiseDataSegmentsSet - ](T_TFlex_Model_Model3D_Geometry_SurfacePiecewiseData_SegmentsSet.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)