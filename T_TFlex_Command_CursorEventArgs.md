

Руководство по T-FLEX CAD Open API

# CursorEventArgs - класс  
    
Базовый класс аргументов событий, возникающих при манипуляциях с курсором

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlex.CommandCommandEventArgs](T_TFlex_Command_CommandEventArgs.md) TFlex.CommandCursorEventArgs [TFlex.CommandKeyEventArgs](T_TFlex_Command_KeyEventArgs.md) [TFlex.CommandMouseEventArgs](T_TFlex_Command_MouseEventArgs.md) [TFlex.CommandSelectEventArgs](T_TFlex_Command_SelectEventArgs.md)

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class CursorEventArgs : CommandEventArgs
```
```vb
Public MustInherit Class CursorEventArgs
	Inherits CommandEventArgs
```
```cpp
public ref class CursorEventArgs abstract : public CommandEventArgs
```


Тип CursorEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Document](P_TFlex_Command_CommandEventArgs_Document.md) | Документ, в котором произошло событие(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [DX](P_TFlex_Command_CursorEventArgs_DX.md) | Координата X курсора в координатах графического контекста |
|  | [DY](P_TFlex_Command_CursorEventArgs_DY.md) | Координата Y курсора в координатах графического контекста |
|  | [Graphics](P_TFlex_Command_CommandEventArgs_Graphics.md) | Графический контекст(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [GX](P_TFlex_Command_CursorEventArgs_GX.md) | Координата X курсора в координатах графического контекста с учётом сетки |
|  | [GY](P_TFlex_Command_CursorEventArgs_GY.md) | Координата Y курсора в координатах графического контекста с учётом сетки |
|  | [SelectedGeometry](P_TFlex_Command_CursorEventArgs_SelectedGeometry.md) | Выбранная геометрия объекта |
|  | [SelectedObject](P_TFlex_Command_CursorEventArgs_SelectedObject.md) | Выбранный объект |
|  | [Window](P_TFlex_Command_CommandEventArgs_Window.md) | Вид документа (окно), в котором произошло событие(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [X](P_TFlex_Command_CursorEventArgs_X.md) | Координата X курсора в пикселях |
|  | [Y](P_TFlex_Command_CursorEventArgs_Y.md) | Координата Y курсора в пикселях |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ConvertSelectedObject](M_TFlex_Command_CursorEventArgs_ConvertSelectedObject.md) |  |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)