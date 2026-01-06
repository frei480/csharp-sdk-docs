

Руководство по T-FLEX CAD Open API

# PluginCommand - класс  
    
Реализация функциональности команды приложения

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.CommandFilterOwner](T_TFlex_Command_FilterOwner.md) TFlex.CommandPluginCommand

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class PluginCommand : FilterOwner, 
	IDisposable
```
```vb
Public MustInherit Class PluginCommand
	Inherits FilterOwner
	Implements IDisposable
```
```cpp
public ref class PluginCommand abstract : public FilterOwner, 
	IDisposable
```


Тип PluginCommand предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [PluginCommand](M_TFlex_Command_PluginCommand__ctor.md) | Конструктор команды |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Automenu](P_TFlex_Command_PluginCommand_Automenu.md) | Автоменю команды |
|  | [DisplayNameForError](P_TFlex_Command_PluginCommand_DisplayNameForError.md) | Название команды для отображения в сообщениях об ошибке |
|  | [ID](P_TFlex_Command_PluginCommand_ID.md) | Возвращает зарегестрированный идентификатор команды |
|  | [IsTransparentChangesEnabled](P_TFlex_Command_PluginCommand_IsTransparentChangesEnabled.md) | Разрешает блоку отмены действий оставаться открытым между событиями команды |
|  | [Owner](P_TFlex_Command_PluginCommand_Owner.md) | Получить приложение команды |
|  | [PropertiesWindow](P_TFlex_Command_PluginCommand_PropertiesWindow.md) | Окно свойств команды |
|  | [SelectionFilter](P_TFlex_Command_PluginCommand_SelectionFilter.md) |  |
|  | [SupportedBehavior](P_TFlex_Command_PluginCommand_SupportedBehavior.md) | Поддерживаемое командой поведение |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CreateSelectionFilterButton(Guid, String)](M_TFlex_Command_FilterOwner_CreateSelectionFilterButton.md) | Создать кнопку селекции(Унаследован от [FilterOwner](T_TFlex_Command_FilterOwner.md)) |
|  | [CreateSelectionFilterButton(Guid, String, SelectionFilterButton)](M_TFlex_Command_FilterOwner_CreateSelectionFilterButton_1.md) | Создать кнопку селекции(Унаследован от [FilterOwner](T_TFlex_Command_FilterOwner.md)) |
|  | [CreateSelectionFilterButton(Guid, String, ObjectType)](M_TFlex_Command_FilterOwner_CreateSelectionFilterButton_2.md) | Создать кнопку селекции(Унаследован от [FilterOwner](T_TFlex_Command_FilterOwner.md)) |
|  | [Dispose](M_TFlex_Command_PluginCommand_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов |
|  | [Dispose(Boolean)](M_TFlex_Command_PluginCommand_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом PluginCommand, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnContinue](M_TFlex_Command_PluginCommand_OnContinue.md) | Обработчик завершения выполнения вложенной команды |
|  | [OnExit](M_TFlex_Command_PluginCommand_OnExit.md) | Обработчик выхода из команды |
|  | [OnHideCursor](M_TFlex_Command_PluginCommand_OnHideCursor.md) | **Устарело.** |
|  | [OnInitialize](M_TFlex_Command_PluginCommand_OnInitialize.md) | Обработчик инициализации команды |
|  | [OnKeyPressed](M_TFlex_Command_PluginCommand_OnKeyPressed.md) | Обработчик нажатия клавиши на клавиатуре или кнопки автоменю |
|  | [OnKeyUp](M_TFlex_Command_PluginCommand_OnKeyUp.md) |  |
|  | [OnMouseMove](M_TFlex_Command_PluginCommand_OnMouseMove.md) | Обработчик перемещения курсора мыши |
|  | [OnSelect](M_TFlex_Command_PluginCommand_OnSelect.md) | Фильтр выбираемых объектов |
|  | [OnSelectionFilterButtonClick(Int32)](M_TFlex_Command_FilterOwner_OnSelectionFilterButtonClick.md) | Для внутреннего использования(Унаследован от [FilterOwner](T_TFlex_Command_FilterOwner.md)) |
|  | [OnSelectionFilterButtonClick(SelectionFilterButtonClickEventArgs)](M_TFlex_Command_FilterOwner_OnSelectionFilterButtonClick_2.md) | Вызывает событие [SelectionFilterButtonClick](E_TFlex_Command_FilterOwner_SelectionFilterButtonClick.md)(Унаследован от [FilterOwner](T_TFlex_Command_FilterOwner.md)) |
|  | [OnSelectionFilterButtonClick(Int32, IntPtr)](M_TFlex_Command_FilterOwner_OnSelectionFilterButtonClick_1.md) | Для внутреннего использования(Унаследован от [FilterOwner](T_TFlex_Command_FilterOwner.md)) |
|  | [OnShowCursor](M_TFlex_Command_PluginCommand_OnShowCursor.md) | Динамическая отрисовка курсора |
|  | [PassSelected](M_TFlex_Command_PluginCommand_PassSelected.md) | Передать ранее выбранный с помощью метода [SelectByEvent(CursorEventArgs, Boolean)](M_TFlex_Command_PluginCommand_SelectByEvent.md) объект системе. |
|  | [RemoveOwnSelectionFilterButtons](M_TFlex_Command_FilterOwner_RemoveOwnSelectionFilterButtons.md) | Удалить все созданные этим объектом кнопки селекции(Унаследован от [FilterOwner](T_TFlex_Command_FilterOwner.md)) |
|  | [ResetSelectedObject](M_TFlex_Command_PluginCommand_ResetSelectedObject.md) | Отменить выбор последнего объекта |
|  | [Run(View)](M_TFlex_Command_PluginCommand_Run.md) | Запустить команду на выполнение |
|  | [Run(View, Boolean)](M_TFlex_Command_PluginCommand_Run_1.md) | Запустить команду на выполнение |
|  | [SelectByEvent](M_TFlex_Command_PluginCommand_SelectByEvent.md) | Функция выбора объекта |
|  | [Terminate](M_TFlex_Command_PluginCommand_Terminate.md) | Завершить выполнение команды |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Continue](E_TFlex_Command_PluginCommand_Continue.md) | Событие завершения выполнения вложенной команды |
|  | [Exit](E_TFlex_Command_PluginCommand_Exit.md) | Событие завершения выполнения команды |
|  | [HideCursor](E_TFlex_Command_PluginCommand_HideCursor.md) | **Устарело.** |
|  | [Initialize](E_TFlex_Command_PluginCommand_Initialize.md) | Событие инициализации команды |
|  | [KeyPressed](E_TFlex_Command_PluginCommand_KeyPressed.md) | Событие, возникающее при нажатии клавиши клавиатуры или кнопки автоменю |
|  | [KeyUp](E_TFlex_Command_PluginCommand_KeyUp.md) |  |
|  | [MouseMove](E_TFlex_Command_PluginCommand_MouseMove.md) | Событие, возникающее при перемещении курсора |
|  | [Select](E_TFlex_Command_PluginCommand_Select.md) | Событие, возникающее при выборе объекта |
|  | [SelectionFilterButtonClick](E_TFlex_Command_FilterOwner_SelectionFilterButtonClick.md) | (Унаследован от [FilterOwner](T_TFlex_Command_FilterOwner.md)) |
|  | [ShowCursor](E_TFlex_Command_PluginCommand_ShowCursor.md) | Событие, возникающее при прорисовке динамического курсора при перемещении мыши |
  
При получении сообщения через функцию [!:TFlex::Plugin::OnCommand(TFlex.Model.Document, System.UInt32)] приложение конструирует объект данного класса и запускает его на выполнение при помощи функции Run. После этого до завершения данной команды или запуска другой команды сообщения Windows транслируются в вызовы функция данного класса.

#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)