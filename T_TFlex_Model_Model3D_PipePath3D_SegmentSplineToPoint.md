

Руководство по T-FLEX CAD Open API

# PipePath3DSegmentSplineToPoint - класс  
    
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3DPipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md) TFlex.Model.Model3DPipePath3DSegmentSplineToPoint

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class SegmentSplineToPoint : PipePath3DBaseSegment
```




Тип PipePath3DSegmentSplineToPoint предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [CountPoints](P_TFlex_Model_Model3D_PipePath3D_BaseSegment_CountPoints.md) | Количество точке в участке(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [Degree](P_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_Degree.md) | Управляет степенью сплайна |
|  | [Reverse](P_TFlex_Model_Model3D_PipePath3D_BaseSegment_Reverse.md) | Разворачивает участок пути(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [Type](P_TFlex_Model_Model3D_PipePath3D_BaseSegment_Type.md) | Тип участка пути(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddBeginPoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_AddBeginPoint.md) | Добавить точку в начало |
|  | [AddEndPoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_AddEndPoint.md) | Добавить точку в конец |
|  | [AddPoint_begin](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_AddPoint_begin.md) | **Устарело.** Добавить точку в начало |
|  | [AddPoint_end](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_AddPoint_end.md) | **Устарело.** Добавить точку в конец |
|  | [Equal](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_Equal.md) | Сравнить два сегмента(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetBeginPoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_GetBeginPoint.md) | Вернуть первую точку |
|  | [GetEndPoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_GetEndPoint.md) | Вернуть последнюю точку |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetNextPoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_GetNextPoint.md) | Вернуть следующую точку |
|  | [GetPoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_GetPoint.md) | Вернуть точку по индексу |
|  | [GetPrevPoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_GetPrevPoint.md) | Вернуть предыдущую точку |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InsertAfterPoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_InsertAfterPoint.md) | Вставить новую точку после точки pPoint |
|  | [InsertBeforePoint](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_InsertBeforePoint.md) | Вставить новую точку перед точки pPoint |
|  | [InsertPoint_after](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_InsertPoint_after.md) | **Устарело.** Вставить новую точку после точки pPoint |
|  | [InsertPoint_before](M_TFlex_Model_Model3D_PipePath3D_SegmentSplineToPoint_InsertPoint_before.md) | **Устарело.** Вставить новую точку перед точки pPoint |
|  | [IsBeginTangentPossible](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_IsBeginTangentPossible.md) | Возможность касательной в начале участка(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [IsEndTangentPossible](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_IsEndTangentPossible.md) | Возможность касательной в конце участка(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemovePoint(PipePath3DBasePoint)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_RemovePoint_1.md) | Удалить точку(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [RemovePoint(Int32)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_RemovePoint.md) | Удалить точку по индексу(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [SetBeginTangent(Boolean, Boolean)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_SetBeginTangent.md) | Управление касательной в начале участка(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [SetBeginTangent(Double, Boolean)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_SetBeginTangent_1.md) | Управление акмплитудой касательной в начале участка(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [SetEndTangent(Boolean, Boolean)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_SetEndTangent.md) | Управление касательной в конце участка(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [SetEndTangent(Double, Boolean)](M_TFlex_Model_Model3D_PipePath3D_BaseSegment_SetEndTangent_1.md) | Управление акмплитудой касательной в конце участка(Унаследован от [PipePath3DBaseSegment](T_TFlex_Model_Model3D_PipePath3D_BaseSegment.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)