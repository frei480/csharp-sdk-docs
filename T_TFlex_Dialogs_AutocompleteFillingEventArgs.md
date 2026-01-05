

Руководство по T-FLEX CAD Open API

# AutocompleteFillingEventArgs - класс  
  
---  
  
Событие автодополнения для InputControlBase

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlex.DialogsBaseEventArgs](T_TFlex_Dialogs_BaseEventArgs.md) TFlex.DialogsAutocompleteFillingEventArgs

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public class AutocompleteFillingEventArgs : BaseEventArgs
```
```vb
Public Class AutocompleteFillingEventArgs
	Inherits BaseEventArgs
```
```cpp
public ref class AutocompleteFillingEventArgs : public BaseEventArgs
```


Тип AutocompleteFillingEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [CompletingText](P_TFlex_Dialogs_AutocompleteFillingEventArgs_CompletingText.md) | Возвращает строку, которую нужно дополнить |
|  | [Handled](P_TFlex_Dialogs_BaseEventArgs_Handled.md) | Помечает событие как обработанное(Унаследован от [BaseEventArgs](T_TFlex_Dialogs_BaseEventArgs.md)) |
|  | [IncludeDefaultItems](P_TFlex_Dialogs_AutocompleteFillingEventArgs_IncludeDefaultItems.md) | Возвращает true, если значение нужно в результирующий список добавлять элементы по умолчанию |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddCustomItem](M_TFlex_Dialogs_AutocompleteFillingEventArgs_AddCustomItem.md) | Добавить пользовательский элемент автодополнения |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)