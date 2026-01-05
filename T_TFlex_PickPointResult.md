

Руководство по T-FLEX CAD Open API

# PickPointResult - класс  
  
---  
  
Выходные параметры метода PickPoint

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlexPickPointResult

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class PickPointResult
```
```vb
Public NotInheritable Class PickPointResult
```
```cpp
public ref class PickPointResult sealed
```


Тип PickPointResult предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [IsOK](P_TFlex_PickPointResult_IsOK.md) | Признак успешного завершения выбора точки или объекта. Если данный параметр равен false, то макрос или команда, вызвавшая метод PickPoint должен завершить работу. Иначе возможны сбои в работе системы. |
|  | [Key](P_TFlex_PickPointResult_Key.md) | Код клавиши, которая была нажата пользователем |
|  | [ModelPoint](P_TFlex_PickPointResult_ModelPoint.md) | Выбранная точка в системе координат модели, с учётом масштаба текущей страницы |
|  | [PaperPoint](P_TFlex_PickPointResult_PaperPoint.md) | Выбранная точка в системе координат бумаги, без учёта масштаба текущей страницы |
|  | [Point](P_TFlex_PickPointResult_Point.md) | Выбранная точка |
|  | [SelectedObject](P_TFlex_PickPointResult_SelectedObject.md) | Объект документа, который был выбран в процессе ввода точки |
|  | [View](P_TFlex_PickPointResult_View.md) | Вид документа, в котором был произведён ввод точки |
|  | [X](P_TFlex_PickPointResult_X.md) | Координата X выбранной точки |
|  | [Y](P_TFlex_PickPointResult_Y.md) | Координата Y выбранной точки |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex - пространство имён](N_TFlex.md)