

Руководство по T-FLEX CAD Open API

# BaseGenerator - класс  
    
Базовый класс для всех генераторов

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometryBaseGenerator [TFlex.Model.Model3D.GeometryBodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BaseGenerator : IDisposable
```
```vb
Public MustInherit Class BaseGenerator
	Implements IDisposable
```
```cpp
public ref class BaseGenerator abstract : IDisposable
```


Тип BaseGenerator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BaseGenerator](M_TFlex_Model_Model3D_Geometry_BaseGenerator__ctor.md) | Конструктор для задания генератора |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [LastResult](P_TFlex_Model_Model3D_Geometry_BaseGenerator_LastResult.md) | Результат |
|  | [Proxy](P_TFlex_Model_Model3D_Geometry_BaseGenerator_Proxy.md) | Получить внешнее приложение, для которого генерируется результат |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose.md) | Освобождает все ресурсы, используемые объектом BaseGenerator |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом BaseGenerator, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Run](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Run.md) | Основная функция генерации геометрических результатов |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)