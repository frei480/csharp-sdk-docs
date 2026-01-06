

Руководство по T-FLEX CAD Open API

# LoftGenerator - класс  
    
Генератор лофтинга

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryBaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md) [TFlex.Model.Model3D.GeometryBodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md) TFlex.Model.Model3D.GeometryLoftGenerator

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class LoftGenerator : BodyGenerator
```
```vb
Public Class LoftGenerator
	Inherits BodyGenerator
```
```cpp
public ref class LoftGenerator : public BodyGenerator
```


Тип LoftGenerator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [LoftGenerator](M_TFlex_Model_Model3D_Geometry_LoftGenerator__ctor.md) | Конструктор для задания базовых объектов |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [LastResult](P_TFlex_Model_Model3D_Geometry_BaseGenerator_LastResult.md) | Результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Proxy](P_TFlex_Model_Model3D_Geometry_BaseGenerator_Proxy.md) | Получить внешнее приложение, для которого генерируется результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Result](P_TFlex_Model_Model3D_Geometry_BodyGenerator_Result.md) | Получить множество результирующих тел(Унаследован от [BodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose.md) | (Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_LoftGenerator_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом LoftGenerator, а при необходимости освобождает также управляемые ресурсы(Переопределяет [BaseGeneratorDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose_1.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Run](M_TFlex_Model_Model3D_Geometry_LoftGenerator_Run.md) | Функция генерации сглаживания(Переопределяет [BaseGeneratorRun](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Run.md)) |
|  | [SetClose](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetClose.md) | Функция задаёт замкнутось лофтинга в направлении V |
|  | [SetCondType](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetCondType.md) | Функция задаёт граничное условие в начале-конце лофтинга |
|  | [SetFApex](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetFApex.md) | Функция устанавливает точку начала лофтинга в качестве первого профиля |
|  | [SetFApexDir](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetFApexDir.md) | Функция устанавливает задающию нормаль к касательной плоскости вершинного лофтинга |
|  | [SetFirstBody](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetFirstBody.md) | Функция тело с которого берутся касательные для начального профиля |
|  | [SetFmodul](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetFmodul.md) | Функция устанавливает модуль касательных в начале лофтинга |
|  | [SetLastBody](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetLastBody.md) | Функция тело с которого берутся касательные для конечного профиля |
|  | [SetPath](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetPath.md) | Функция устанавливает "осевой" путь для выполнения лофтинга с путём |
|  | [SetProfileU](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetProfileU.md) | Функция задаёт профиль в направлении U |
|  | [SetProfileV](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetProfileV.md) | Функция задаёт профиль в направлении V |
|  | [SetSApex](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetSApex.md) | Функция устанавливает точку завершения лофтинга в качестве последнего профиля |
|  | [SetSApexDir](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetSApexDir.md) | Функция устанавливает задающию нормаль к касательной плоскости вершинного лофтинга |
|  | [SetSimpl](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetSimpl.md) | Функция задаёт режим упрощения результирующей геометрии |
|  | [SetSmodul](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetSmodul.md) | Функция устанавливает модуль касательных в конце лофтинга |
|  | [SetSyncVertex](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetSyncVertex.md) | Функция устанавливает вершину соответствия между профилями |
|  | [SetThicken](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetThicken.md) | Функция задаёт величины отступов для создания оболочечного тела |
|  | [SetTolerance](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetTolerance.md) | Функция задаёт точность аппроксимации |
|  | [SetType](M_TFlex_Model_Model3D_Geometry_LoftGenerator_SetType.md) | Функция задаёт тип лофтинга (линейчатый или сплайновый) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)