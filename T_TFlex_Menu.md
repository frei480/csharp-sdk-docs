

Руководство по T-FLEX CAD Open API

# Menu - класс  
    
Класс меню

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlexMenu

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class Menu : IDisposable
```




Тип Menu предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Menu](M_TFlex_Menu__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Append(Int32, String, Plugin)](M_TFlex_Menu_Append_1.md) | Добавить пункт меню |
|  | [Append(Int32, String, Boolean, Boolean, Plugin)](M_TFlex_Menu_Append.md) | Добавить пункт меню |
|  | [AppendSeparator](M_TFlex_Menu_AppendSeparator.md) | Добавить разделитель в меню |
|  | [AppendSubMenu](M_TFlex_Menu_AppendSubMenu.md) | Добавить подменю |
|  | [AppendSystemCommand(Int32)](M_TFlex_Menu_AppendSystemCommand.md) | Добавить пункт меню |
|  | [AppendSystemCommand(Int32, String)](M_TFlex_Menu_AppendSystemCommand_1.md) | Добавить пункт меню |
|  | [CreatePopup](M_TFlex_Menu_CreatePopup.md) | Создать контекстное меню |
|  | [DeleteByCommand](M_TFlex_Menu_DeleteByCommand.md) | Удалить команду по идентификатору |
|  | [DeleteByIndex](M_TFlex_Menu_DeleteByIndex.md) | Удалить команду по порядковому номеру |
|  | [Dispose](M_TFlex_Menu_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetCaption](M_TFlex_Menu_GetCaption.md) | Получить название пункта меню команды по её порядковому номеру |
|  | [GetCommand](M_TFlex_Menu_GetCommand.md) | Получить идентификатор команды по её порядковому номеру в меню |
|  | [GetCount](M_TFlex_Menu_GetCount.md) | Получить общее количество пунктов меню |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetSubMenu](M_TFlex_Menu_GetSubMenu.md) | Получить подменю по её порядковому номеру в меню |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Insert](M_TFlex_Menu_Insert.md) | Вставить пункт меню |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex - пространство имён](N_TFlex.md)