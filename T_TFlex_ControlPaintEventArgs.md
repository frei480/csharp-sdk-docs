

Руководство по T-FLEX CAD Open API

# ControlPaintEventArgs - класс  
  
---  
  
Класс аргументов событий, возникающих при отрисовке

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlexControlEventArgs](T_TFlex_ControlEventArgs.md) TFlexControlPaintEventArgs

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class ControlPaintEventArgs : ControlEventArgs
```
```vb
Public Class ControlPaintEventArgs
	Inherits ControlEventArgs
```
```cpp
public ref class ControlPaintEventArgs : public ControlEventArgs
```


Тип ControlPaintEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Cancel](P_TFlex_ControlEventArgs_Cancel.md) | Вызывать обработку базового метода(Унаследован от [ControlEventArgs](T_TFlex_ControlEventArgs.md)) |
|  | [Graphics](P_TFlex_ControlPaintEventArgs_Graphics.md) | Графический контекст |
|  | [ModelX](P_TFlex_ControlEventArgs_ModelX.md) | Координата X положения курсора мыши на момент возникновения события(в единицах измерения чертежа)(Унаследован от [ControlEventArgs](T_TFlex_ControlEventArgs.md)) |
|  | [ModelY](P_TFlex_ControlEventArgs_ModelY.md) | Координата Y положения курсора мыши на момент возникновения события(в единицах измерения чертежа)(Унаследован от [ControlEventArgs](T_TFlex_ControlEventArgs.md)) |
|  | [x](P_TFlex_ControlEventArgs_x.md) | Координата X положения курсора мыши на момент возникновения события(в пикселях)(Унаследован от [ControlEventArgs](T_TFlex_ControlEventArgs.md)) |
|  | [y](P_TFlex_ControlEventArgs_y.md) | Координата Y положения курсора мыши на момент возникновения события(в пикселях)(Унаследован от [ControlEventArgs](T_TFlex_ControlEventArgs.md)) |
  
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