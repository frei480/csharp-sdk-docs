

Руководство по T-FLEX CAD Open API

# InitializeEventArgs - класс  
    
Класс аргументов события, возникающего при инициализации команды приложения

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlex.CommandCommandEventArgs](T_TFlex_Command_CommandEventArgs.md) TFlex.CommandInitializeEventArgs

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class InitializeEventArgs : CommandEventArgs
```
```vb
Public NotInheritable Class InitializeEventArgs
	Inherits CommandEventArgs
```
```cpp
public ref class InitializeEventArgs sealed : public CommandEventArgs
```


Тип InitializeEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Document](P_TFlex_Command_CommandEventArgs_Document.md) | Документ, в котором произошло событие(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [Graphics](P_TFlex_Command_CommandEventArgs_Graphics.md) | Графический контекст(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [Window](P_TFlex_Command_CommandEventArgs_Window.md) | Вид документа (окно), в котором произошло событие(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)