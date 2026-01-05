

Руководство по T-FLEX CAD Open API

# Contour - класс  
  
---  
  
Контур штриховки/заливки

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model2DContour

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class Contour : IEnumerable<ContourSegment>
```
```vb
Public NotInheritable Class Contour
	Implements IEnumerable(Of ContourSegment)
```
```cpp
public ref class Contour sealed : IEnumerable<ContourSegment^>
```


Тип Contour предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [SegmentCount](P_TFlex_Model_Model2D_Contour_SegmentCount.md) | Количество сегментов контура штриховки |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [DeleteAllSegments](M_TFlex_Model_Model2D_Contour_DeleteAllSegments.md) | Удаление всех сегментов контура |
|  | [DeleteSegment](M_TFlex_Model_Model2D_Contour_DeleteSegment.md) | Удаление сегмента контура по указанному индексу |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_Model_Model2D_Contour_GetEnumerator.md) | Получить перечилитель |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetSegment](M_TFlex_Model_Model2D_Contour_GetSegment.md) | Получение сегмента контура по указанному индексу |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)