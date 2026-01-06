

Руководство по T-FLEX CAD Open API

# MouseEventArgs - класс  
    
Класс аргументов событий, возникающих при перемещении мыши

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlex.CommandCommandEventArgs](T_TFlex_Command_CommandEventArgs.md) [TFlex.CommandCursorEventArgs](T_TFlex_Command_CursorEventArgs.md) TFlex.CommandMouseEventArgs

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class MouseEventArgs : CursorEventArgs
```
```vb
Public NotInheritable Class MouseEventArgs
	Inherits CursorEventArgs
```
```cpp
public ref class MouseEventArgs sealed : public CursorEventArgs
```


Тип MouseEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [CursorAction](P_TFlex_Command_MouseEventArgs_CursorAction.md) | Режим динамической прорисовки курсора |
|  | [Document](P_TFlex_Command_CommandEventArgs_Document.md) | Документ, в котором произошло событие(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [DX](P_TFlex_Command_CursorEventArgs_DX.md) | Координата X курсора в координатах графического контекста(Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
|  | [DY](P_TFlex_Command_CursorEventArgs_DY.md) | Координата Y курсора в координатах графического контекста(Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
|  | [Graphics](P_TFlex_Command_CommandEventArgs_Graphics.md) | Графический контекст(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [GX](P_TFlex_Command_CursorEventArgs_GX.md) | Координата X курсора в координатах графического контекста с учётом сетки(Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
|  | [GY](P_TFlex_Command_CursorEventArgs_GY.md) | Координата Y курсора в координатах графического контекста с учётом сетки(Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
|  | [SelectedGeometry](P_TFlex_Command_CursorEventArgs_SelectedGeometry.md) | Выбранная геометрия объекта(Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
|  | [SelectedObject](P_TFlex_Command_CursorEventArgs_SelectedObject.md) | Выбранный объект(Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
|  | [Window](P_TFlex_Command_CommandEventArgs_Window.md) | Вид документа (окно), в котором произошло событие(Унаследован от [CommandEventArgs](T_TFlex_Command_CommandEventArgs.md)) |
|  | [X](P_TFlex_Command_CursorEventArgs_X.md) | Координата X курсора в пикселях(Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
|  | [Y](P_TFlex_Command_CursorEventArgs_Y.md) | Координата Y курсора в пикселях(Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ConvertSelectedObject](M_TFlex_Command_CursorEventArgs_ConvertSelectedObject.md) | (Унаследован от [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)