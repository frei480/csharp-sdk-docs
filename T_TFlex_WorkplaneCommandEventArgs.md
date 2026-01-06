

Руководство по T-FLEX CAD Open API

# WorkplaneCommandEventArgs - класс  
    
Класс, содержащий данные о событии - вызвана команда управления рабочими плоскостями

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlexPluginEventArgs](T_TFlex_PluginEventArgs.md) [TFlexDocumentEventArgs](T_TFlex_DocumentEventArgs.md) TFlexWorkplaneCommandEventArgs

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class WorkplaneCommandEventArgs : DocumentEventArgs
```
```vb
Public Class WorkplaneCommandEventArgs
	Inherits DocumentEventArgs
```
```cpp
public ref class WorkplaneCommandEventArgs : public DocumentEventArgs
```


Тип WorkplaneCommandEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Cancel](P_TFlex_PluginEventArgs_Cancel.md) | true, если действие было отменено пользователем или системой(Унаследован от [PluginEventArgs](T_TFlex_PluginEventArgs.md)) |
|  | [Command](P_TFlex_WorkplaneCommandEventArgs_Command.md) | Идентификатор команды |
|  | [Count](P_TFlex_WorkplaneCommandEventArgs_Count.md) | Количество создаваемых плоскостей |
|  | [Document](P_TFlex_DocumentEventArgs_Document.md) | Документ, в котором произошло данное событие(Унаследован от [DocumentEventArgs](T_TFlex_DocumentEventArgs.md)) |
|  | [IsUseStep](P_TFlex_WorkplaneCommandEventArgs_IsUseStep.md) | true, если должно быть использовано значение шага |
|  | [Step](P_TFlex_WorkplaneCommandEventArgs_Step.md) | Шаг плоскостей или расстояние между двумя плоскостями |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex - пространство имён](N_TFlex.md)