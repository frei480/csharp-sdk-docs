

Руководство по T-FLEX CAD Open API

# FaceFaceBlendGenerator - класс  
  
---  
  
Генератор сглаживания граней

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryBaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md) [TFlex.Model.Model3D.GeometryBodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md) TFlex.Model.Model3D.GeometryFaceFaceBlendGenerator

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class FaceFaceBlendGenerator : BodyGenerator
```
```vb
Public Class FaceFaceBlendGenerator
	Inherits BodyGenerator
```
```cpp
public ref class FaceFaceBlendGenerator : public BodyGenerator
```


Тип FaceFaceBlendGenerator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [FaceFaceBlendGenerator](M_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator__ctor.md) | Конструктор для задания базовых объектов сглаживания |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [LastResult](P_TFlex_Model_Model3D_Geometry_BaseGenerator_LastResult.md) | Результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Proxy](P_TFlex_Model_Model3D_Geometry_BaseGenerator_Proxy.md) | Получить внешнее приложение, для которого генерируется результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Ratio](P_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_Ratio.md) | Отношение сторон для сглаживания постоянной ширины |
|  | [Result](P_TFlex_Model_Model3D_Geometry_BodyGenerator_Result.md) | Получить множество результирующих тел(Унаследован от [BodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md)) |
|  | [RF](P_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_RF.md) | Радиус сглаживания для сглаживания с постоянным радиусом |
|  | [Softness](P_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_Softness.md) | Коэффициент "мягкости" для сглаживания с непрерывностью по кривизне |
|  | [Spine](P_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_Spine.md) | Направляющая кривая |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddEdgeToBorder](M_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_AddEdgeToBorder.md) | Функция добавляет ограничительное ребро в список таких рёбер |
|  | [AddFaceToLeftWall](M_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_AddFaceToLeftWall.md) | Функция добавляет грань в левую стенку |
|  | [AddFaceToRightWall](M_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_AddFaceToRightWall.md) | Функция добавляет грань в правую стенку |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose.md) | (Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом FaceFaceBlendGenerator, а при необходимости освобождает также управляемые ресурсы(Переопределяет [BaseGeneratorDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose_1.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FlushFacesAndEdges](M_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_FlushFacesAndEdges.md) | Функция сбрасывает заданные данные |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Run](M_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator_Run.md) | Функция генерации сглаживания(Переопределяет [BaseGeneratorRun](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Run.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)