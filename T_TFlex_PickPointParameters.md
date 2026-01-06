

Руководство по T-FLEX CAD Open API

# PickPointParameters - класс  
    
Входные параметры метода PickPoint

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlexPickPointParameters

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class PickPointParameters
```




Тип PickPointParameters предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [PickPointParameters](M_TFlex_PickPointParameters__ctor.md) | Инициализирует новый экземпляр класса PickPointParameters |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Automenu](P_TFlex_PickPointParameters_Automenu.md) | Автоменю, которое будет выведено на экран в процессе выбора точки |
|  | [CanCreateNode](P_TFlex_PickPointParameters_CanCreateNode.md) | Признак того, что в процессе выбора элементов модели возможно создание новых узлов |
|  | [Filter](P_TFlex_PickPointParameters_Filter.md) | Фильтр, позволяющий в процессе выбора точки выбирать также элементы модели |
|  | [Prompt](P_TFlex_PickPointParameters_Prompt.md) | Подсказка, которая появится в статусной строке. В случае, если подсказка не задана, она останется без изменений |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [MouseMove](E_TFlex_PickPointParameters_MouseMove.md) | Cобытие перемещения мыши при вызове метода PickPoint |
  
#### Ссылки

[TFlex - пространство имён](N_TFlex.md)