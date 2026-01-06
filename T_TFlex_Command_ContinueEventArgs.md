

Руководство по T-FLEX CAD Open API

# ContinueEventArgs - класс  
    
Класс аргументов события завершения выполнения вложенной команды приложения

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlex.CommandCommandEventArgs](T_TFlex_Command_CommandEventArgs.md) TFlex.CommandContinueEventArgs

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class ContinueEventArgs : CommandEventArgs
```




Тип ContinueEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Document](P_TFlex_Command_CommandEventArgs_Document.md) | Документ, в котором произошло событие(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [Graphics](P_TFlex_Command_CommandEventArgs_Graphics.md) | Графический контекст(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [PreviousCommand](P_TFlex_Command_ContinueEventArgs_PreviousCommand.md) | Вложенная команда, которая завершилась |
|  | [Result](P_TFlex_Command_ContinueEventArgs_Result.md) | Объект, который был передан из вложенной команды |
|  | [Window](P_TFlex_Command_CommandEventArgs_Window.md) | Вид документа (окно), в котором произошло событие(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Вложенной командой называется команда, функция TFlex.Command.PluginCommand.Run(TFlex.Model.View, bool) которой вызвана внутри обработчика выполнения другой (вызывающей) команды

#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)