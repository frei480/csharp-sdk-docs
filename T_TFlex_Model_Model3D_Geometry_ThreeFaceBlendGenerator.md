

Руководство по T-FLEX CAD Open API

# ThreeFaceBlendGenerator - класс  
    
Генератор трёхгранного сглаживания

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryBaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md) [TFlex.Model.Model3D.GeometryBodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md) TFlex.Model.Model3D.GeometryThreeFaceBlendGenerator

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class ThreeFaceBlendGenerator : BodyGenerator
```
```vb
Public Class ThreeFaceBlendGenerator
	Inherits BodyGenerator
```
```cpp
public ref class ThreeFaceBlendGenerator : public BodyGenerator
```


Тип ThreeFaceBlendGenerator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ThreeFaceBlendGenerator](M_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator__ctor.md) | Конструктор для задания базовых объектов сглаживания |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [LastResult](P_TFlex_Model_Model3D_Geometry_BaseGenerator_LastResult.md) | Результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Proxy](P_TFlex_Model_Model3D_Geometry_BaseGenerator_Proxy.md) | Получить внешнее приложение, для которого генерируется результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Result](P_TFlex_Model_Model3D_Geometry_BodyGenerator_Result.md) | Получить множество результирующих тел(Унаследован от [BodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md)) |
|  | [Spine](P_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator_Spine.md) | Направляющая кривая |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddFaceToCenterWall](M_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator_AddFaceToCenterWall.md) | Функция добавляет грань в список для центральной стенки |
|  | [AddFaceToLeftWall](M_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator_AddFaceToLeftWall.md) | Функция добавляет грань в список для левой стенки |
|  | [AddFaceToRightWall](M_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator_AddFaceToRightWall.md) | Функция добавляет грань в список для правой стенки |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose.md) | (Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом ThreeFaceBlendGenerator, а при необходимости освобождает также управляемые ресурсы(Переопределяет [BaseGeneratorDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose_1.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Run](M_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator_Run.md) | Функция генерации сглаживания(Переопределяет [BaseGeneratorRun](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Run.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)