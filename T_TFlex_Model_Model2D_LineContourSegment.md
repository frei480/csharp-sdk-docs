

Руководство по T-FLEX CAD Open API

# LineContourSegment - класс  
  
---  
  
Сегмент контура штриховки, являющийся отрезком.

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model2DContourSegment](T_TFlex_Model_Model2D_ContourSegment.md) TFlex.Model.Model2DLineContourSegment

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class LineContourSegment : ContourSegment
```
```vb
Public Class LineContourSegment
	Inherits ContourSegment
```
```cpp
public ref class LineContourSegment : public ContourSegment
```


Тип LineContourSegment предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [LineContourSegment(Contour)](M_TFlex_Model_Model2D_LineContourSegment__ctor.md) | Конструктор, добавляющий сегмент в конец контура |
|  | [LineContourSegment(Contour, Int32)](M_TFlex_Model_Model2D_LineContourSegment__ctor_1.md) | Конструктор, вставляющий сегмент в контур по указанному индексу |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Geometry](P_TFlex_Model_Model2D_ContourSegment_Geometry.md) | Геометрия сегмента контура(Унаследован от [ContourSegment](T_TFlex_Model_Model2D_ContourSegment.md)) |
|  | [GeometryType](P_TFlex_Model_Model2D_ContourSegment_GeometryType.md) | Тип геометрии сегмента контура(Унаследован от [ContourSegment](T_TFlex_Model_Model2D_ContourSegment.md)) |
|  | [IsCounterclockwise](P_TFlex_Model_Model2D_ContourSegment_IsCounterclockwise.md) | Направление сегмента контура против часовой стрелки(Унаследован от [ContourSegment](T_TFlex_Model_Model2D_ContourSegment.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [m_Contour](F_TFlex_Model_Model2D_ContourSegment_m_Contour.md) | Для внутреннего использования(Унаследован от [ContourSegment](T_TFlex_Model_Model2D_ContourSegment.md)) |
|  | [m_Handle](F_TFlex_Model_Model2D_ContourSegment_m_Handle.md) | Для внутреннего использования(Унаследован от [ContourSegment](T_TFlex_Model_Model2D_ContourSegment.md)) |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)