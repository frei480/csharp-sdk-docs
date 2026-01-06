

Руководство по T-FLEX CAD Open API

# FilterOwner - класс  
    
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.CommandFilterOwner [TFlex.CommandCommandState](T_TFlex_Command_CommandState.md) [TFlex.CommandCustomCommand](T_TFlex_Command_CustomCommand.md) [TFlex.CommandPluginCommand](T_TFlex_Command_PluginCommand.md)

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class FilterOwner : IFilterOwner
```




Тип FilterOwner предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [FilterOwner](M_TFlex_Command_FilterOwner__ctor.md) | Инициализирует новый экземпляр класса FilterOwner |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CreateSelectionFilterButton(Guid, String)](M_TFlex_Command_FilterOwner_CreateSelectionFilterButton.md) | Создать кнопку селекции |
|  | [CreateSelectionFilterButton(Guid, String, SelectionFilterButton)](M_TFlex_Command_FilterOwner_CreateSelectionFilterButton_1.md) | Создать кнопку селекции |
|  | [CreateSelectionFilterButton(Guid, String, ObjectType)](M_TFlex_Command_FilterOwner_CreateSelectionFilterButton_2.md) | Создать кнопку селекции |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnSelectionFilterButtonClick(Int32)](M_TFlex_Command_FilterOwner_OnSelectionFilterButtonClick.md) | Для внутреннего использования |
|  | [OnSelectionFilterButtonClick(SelectionFilterButtonClickEventArgs)](M_TFlex_Command_FilterOwner_OnSelectionFilterButtonClick_2.md) | Вызывает событие [SelectionFilterButtonClick](E_TFlex_Command_FilterOwner_SelectionFilterButtonClick.md) |
|  | [OnSelectionFilterButtonClick(Int32, IntPtr)](M_TFlex_Command_FilterOwner_OnSelectionFilterButtonClick_1.md) | Для внутреннего использования |
|  | [RemoveOwnSelectionFilterButtons](M_TFlex_Command_FilterOwner_RemoveOwnSelectionFilterButtons.md) | Удалить все созданные этим объектом кнопки селекции |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [SelectionFilterButtonClick](E_TFlex_Command_FilterOwner_SelectionFilterButtonClick.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [GetSelectionFilterButtonState](M_TFlex_Command_FilterOwnerExtensions_GetSelectionFilterButtonState.md) | Получить состояние кнопки селекции(Определяется [FilterOwnerExtensions](T_TFlex_Command_FilterOwnerExtensions.md)) |
|  | [HideAllSelectionFilterButtons](M_TFlex_Command_FilterOwnerExtensions_HideAllSelectionFilterButtons.md) | Скрыть все фильтры селекции(Определяется [FilterOwnerExtensions](T_TFlex_Command_FilterOwnerExtensions.md)) |
|  | [ResumeSelectionFilterNotifications](M_TFlex_Command_FilterOwnerExtensions_ResumeSelectionFilterNotifications.md) | Закончить настройку панели фильтров(Определяется [FilterOwnerExtensions](T_TFlex_Command_FilterOwnerExtensions.md)) |
|  | [SetSelectionFilterButtonState](M_TFlex_Command_FilterOwnerExtensions_SetSelectionFilterButtonState.md) | Установить состояние кнопки селекции(Определяется [FilterOwnerExtensions](T_TFlex_Command_FilterOwnerExtensions.md)) |
|  | [SetSelectionFilterButtonToolTip](M_TFlex_Command_FilterOwnerExtensions_SetSelectionFilterButtonToolTip.md) | Установить подсказку у кнопки селектора(Определяется [FilterOwnerExtensions](T_TFlex_Command_FilterOwnerExtensions.md)) |
|  | [ShowSelectionFilterButton](M_TFlex_Command_FilterOwnerExtensions_ShowSelectionFilterButton.md) | Показать кнопку фильтра селекции(Определяется [FilterOwnerExtensions](T_TFlex_Command_FilterOwnerExtensions.md)) |
|  | [ShowSelectionFilterSet](M_TFlex_Command_FilterOwnerExtensions_ShowSelectionFilterSet.md) | Показать конфигурацию селектора(Определяется [FilterOwnerExtensions](T_TFlex_Command_FilterOwnerExtensions.md)) |
|  | [SuspendSelectionFilterNotifications](M_TFlex_Command_FilterOwnerExtensions_SuspendSelectionFilterNotifications.md) | Начать настройку панели фильтров(Определяется [FilterOwnerExtensions](T_TFlex_Command_FilterOwnerExtensions.md)) |
  
#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)