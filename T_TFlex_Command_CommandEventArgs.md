

Руководство по T-FLEX CAD Open API

# CommandEventArgs - класс  
  
---  
  
Базовый класс аргументов событий, возникающих при манипуляциях с командами приложения

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) TFlex.CommandCommandEventArgs Подробнее

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class CommandEventArgs : EventArgs
```
```vb
Public MustInherit Class CommandEventArgs
	Inherits EventArgs
```
```cpp
public ref class CommandEventArgs abstract : public EventArgs
```


Тип CommandEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Document](P_TFlex_Command_CommandEventArgs_Document.md) | Документ, в котором произошло событие |
|  | [Graphics](P_TFlex_Command_CommandEventArgs_Graphics.md) | Графический контекст |
|  | [Window](P_TFlex_Command_CommandEventArgs_Window.md) | Вид документа (окно), в котором произошло событие |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) TFlex.CommandCommandEventArgs [TFlex.CommandContinueEventArgs](T_TFlex_Command_ContinueEventArgs.md) [TFlex.CommandCursorEventArgs](T_TFlex_Command_CursorEventArgs.md) [TFlex.CommandExitEventArgs](T_TFlex_Command_ExitEventArgs.md) [TFlex.CommandInitializeEventArgs](T_TFlex_Command_InitializeEventArgs.md) [TFlex.CommandPropetiesWindowHeaderButtonPressedEventArgs](T_TFlex_Command_PropetiesWindowHeaderButtonPressedEventArgs.md)