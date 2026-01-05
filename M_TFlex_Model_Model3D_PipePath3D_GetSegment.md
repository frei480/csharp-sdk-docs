

Руководство по T-FLEX CAD Open API

# PipePath3DGetSegment - метод  
  
---  
  
Получить участок

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public PipePath3DBaseSegment GetSegment(
	int indexSegment
)
```
```vb
Public Function GetSegment ( 
	indexSegment As Integer
) As PipePath3DBaseSegment
```
```cpp
public:
PipePath3DBaseSegment^ GetSegment(
	int indexSegment
)
```


#### Параметры

indexSegment [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    

#### Возвращаемое значение

[PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)

Индекс indexSegment должен лежат в интервале от 0 до CountSegments. Возвращаемое значение необходимо преобразовать к соответствующему типу сегмента.

#### Ссылки

[PipePath3D - ](T_TFlex_Model_Model3D_PipePath3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)