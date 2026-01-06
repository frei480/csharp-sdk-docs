

Руководство по T-FLEX CAD Open API

# PipePath3DBaseSegment - класс  
    
Базовый класс участок пути

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3DPipePath3DBaseSegment Подробнее

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BaseSegment
```
```vb
Public MustInherit Class BaseSegment
```
```cpp
public ref class BaseSegment abstract
```


Тип PipePath3DBaseSegment предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [CountPoints](P_TFlex_Model_Model3D_PipePath3D_BaseSegment_CountPoints.md) | Количество точке в участке |
|  | [Reverse](P_TFlex_Model_Model3D_PipePath3D_BaseSegment_Reverse.md) | Разворачивает участок пути |
|  | [Type](P_TFlex_Model_Model3D_PipePath3D_BaseSegment_Type.md) | Тип участка пути |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equal](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_Equal.md) | Сравнить два сегмента |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IsBeginTangentPossible](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_IsBeginTangentPossible.md) | Возможность касательной в начале участка |
|  | [IsEndTangentPossible](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_IsEndTangentPossible.md) | Возможность касательной в конце участка |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemovePoint(PipePath3DBasePoint)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_RemovePoint_1.md) | Удалить точку |
|  | [RemovePoint(Int32)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_RemovePoint.md) | Удалить точку по индексу |
|  | [SetBeginTangent(Boolean, Boolean)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_SetBeginTangent.md) | Управление касательной в начале участка |
|  | [SetBeginTangent(Double, Boolean)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_SetBeginTangent_1.md) | Управление акмплитудой касательной в начале участка |
|  | [SetEndTangent(Boolean, Boolean)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_SetEndTangent.md) | Управление касательной в конце участка |
|  | [SetEndTangent(Double, Boolean)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_SetEndTangent_1.md) | Управление акмплитудой касательной в конце участка |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3DPipePath3DBaseSegment [TFlex.Model.Model3DPipePath3DSegmentOnPath](T_TFlex_Model_Model3D_PipePath3D_SegmentOnPath.md) [TFlex.Model.Model3DPipePath3DSegmentOnSurface](T_TFlex_Model_Model3D_PipePath3D_SegmentOnSurface.md) [TFlex.Model.Model3DPipePath3DSegmentPolyline](T_TFlex_Model_Model3D_PipePath3D_SegmentPolyline.md) [TFlex.Model.Model3DPipePath3DSegmentSplineToPoint](T_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint.md) [TFlex.Model.Model3DPipePath3DSegmentSplineToPolyline](T_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPolyline.md)