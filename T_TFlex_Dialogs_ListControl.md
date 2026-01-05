

Руководство по T-FLEX CAD Open API

# ListControl - класс  
  
---  
  
Элемент управления, отображающий данные в виде списка

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.DialogsUiObject](T_TFlex_Dialogs_UiObject.md) [TFlex.DialogsBaseControl](T_TFlex_Dialogs_BaseControl.md) TFlex.DialogsListControl [TFlex.DialogsSimpleListControl](T_TFlex_Dialogs_SimpleListControl.md)

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public class ListControl : BaseControl
```
```vb
Public Class ListControl
	Inherits BaseControl
```
```cpp
public ref class ListControl : public BaseControl
```


Тип ListControl предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ListControl](M_TFlex_Dialogs_ListControl__ctor.md) | Инициализирует новый экземпляр класса ListControl |
|  | [ListControl(String)](M_TFlex_Dialogs_ListControl__ctor_1.md) | Инициализирует новый экземпляр класса ListControl |
|  | [ListControl(String, ListControlModel)](M_TFlex_Dialogs_ListControl__ctor_2.md) | Инициализирует новый экземпляр класса ListControl |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AutoAddLabelColon](P_TFlex_Dialogs_BaseControl_AutoAddLabelColon.md) | Автоматически добавлять двоеточие к метке(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Buttons](P_TFlex_Dialogs_ListControl_Buttons.md) | Коллекция кнопок, отображаемых контролом |
|  | [Children](P_TFlex_Dialogs_BaseControl_Children.md) | Доступ к дочерним элементам(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [CustomLocalizationId](P_TFlex_Dialogs_BaseControl_CustomLocalizationId.md) | Отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [EditingCell](P_TFlex_Dialogs_ListControl_EditingCell.md) |  |
|  | [EditMode](P_TFlex_Dialogs_ListControl_EditMode.md) | Режим редактирования ячеек ListControl-а |
|  | [Editors](P_TFlex_Dialogs_ListControl_Editors.md) |  |
|  | [ExtendedHintText](P_TFlex_Dialogs_BaseControl_ExtendedHintText.md) | Расширенный текст подсказки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [FullId](P_TFlex_Dialogs_BaseControl_FullId.md) | Полный идентификатор элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GridLinesVisibility](P_TFlex_Dialogs_ListControl_GridLinesVisibility.md) | Режим отображения линий сетки |
|  | [HintDelay](P_TFlex_Dialogs_BaseControl_HintDelay.md) | Задержка показа подсказки в миллисекундах(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintDuration](P_TFlex_Dialogs_BaseControl_HintDuration.md) | Продолжительность показа подсказки в миллисекундах(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintIcon](P_TFlex_Dialogs_BaseControl_HintIcon.md) | Изображение для подсказки. Изображение показывается во всплывающей подсказке.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintText](P_TFlex_Dialogs_BaseControl_HintText.md) | Текст подсказки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HorizontalAlignment](P_TFlex_Dialogs_BaseControl_HorizontalAlignment.md) | Горизонтальное выравнивание элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Id](P_TFlex_Dialogs_BaseControl_Id.md) | Идентификатор элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IndexInParent](P_TFlex_Dialogs_BaseControl_IndexInParent.md) | Индекс в родительском элементе(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsActive](P_TFlex_Dialogs_BaseControl_IsActive.md) | Элемент является текущим активным элементом в форме(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsEditingCell](P_TFlex_Dialogs_ListControl_IsEditingCell.md) |  |
|  | [IsEnabled](P_TFlex_Dialogs_BaseControl_IsEnabled.md) | Элемент включён(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsFocused](P_TFlex_Dialogs_BaseControl_IsFocused.md) | Элемент имеет фокус ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsHierarchyOn](P_TFlex_Dialogs_ListControl_IsHierarchyOn.md) | Включить поддержку иерархии строк. Для задания вложенность задается родительская строка. |
|  | [IsIdMappingOn](P_TFlex_Dialogs_ListControl_IsIdMappingOn.md) | Включить поддержку идентификации строк по id |
|  | [IsReadOnly](P_TFlex_Dialogs_BaseControl_IsReadOnly.md) | Элемент только для чтения(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRequired](P_TFlex_Dialogs_BaseControl_IsRequired.md) | Обязательный параметр. Влияет на отображение элемента.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRequirementMet](P_TFlex_Dialogs_BaseControl_IsRequirementMet.md) | Обязательный параметр заполнен. Связан со свойством IsRequired. Влияет на отображение элемента.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsStretchHeight](P_TFlex_Dialogs_ListControl_IsStretchHeight.md) | Элемент управления растянут по вертикали, чтобы заполнить все доступное пространство. |
|  | [IsVisible](P_TFlex_Dialogs_BaseControl_IsVisible.md) | Элемент видимый(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Label](P_TFlex_Dialogs_BaseControl_Label.md) | Текст метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LabelPadding](P_TFlex_Dialogs_BaseControl_LabelPadding.md) | Выравнивание элемента по меткам(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LabelPosition](P_TFlex_Dialogs_BaseControl_LabelPosition.md) | Положение метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LocalizationMode](P_TFlex_Dialogs_BaseControl_LocalizationMode.md) | Режим локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockBehavior](P_TFlex_Dialogs_BaseControl_LockBehavior.md) | Режим работы чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockMode](P_TFlex_Dialogs_BaseControl_LockMode.md) | Режим отображения чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockPadding](P_TFlex_Dialogs_BaseControl_LockPadding.md) | Выравнивание меток по чекбоксам(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockState](P_TFlex_Dialogs_BaseControl_LockState.md) | Текущее значение чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [MaxHeight](P_TFlex_Dialogs_BaseControl_MaxHeight.md) | Максимальная высота элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [MaxWidth](P_TFlex_Dialogs_BaseControl_MaxWidth.md) | Максимальная ширина элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [MinHeight](P_TFlex_Dialogs_BaseControl_MinHeight.md) | Минимальная высота элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [MinWidth](P_TFlex_Dialogs_BaseControl_MinWidth.md) | Минимальная ширина элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Model](P_TFlex_Dialogs_ListControl_Model.md) | Модель данных списка |
|  | [Parent](P_TFlex_Dialogs_BaseControl_Parent.md) | Родительский элемент(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [PlaceholderText](P_TFlex_Dialogs_BaseControl_PlaceholderText.md) | Замещающий текст(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SelectedRow](P_TFlex_Dialogs_ListControl_SelectedRow.md) | Возвращает индекс первой выбранной строки или -1 |
|  | [SelectedRows](P_TFlex_Dialogs_ListControl_SelectedRows.md) | Коллекция индексов выбранных элементов |
|  | [Tag](P_TFlex_Dialogs_BaseControl_Tag.md) | Пользовательские данные(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Dialogs_BaseControl_Activate.md) | Сделать элемент текущим активным элементом(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [BeginCellEditing(CellInfo)](M_TFlex_Dialogs_ListControl_BeginCellEditing_1.md) |  |
|  | [BeginCellEditing(Int32, Int32)](M_TFlex_Dialogs_ListControl_BeginCellEditing.md) |  |
|  | [CollapseAll](M_TFlex_Dialogs_ListControl_CollapseAll.md) | Свернуть все строки. IsHierarchyOn должно быть true. |
|  | [DisableLocalization](M_TFlex_Dialogs_BaseControl_DisableLocalization.md) | Отключить локализацию данного элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Dispose](M_TFlex_Dialogs_UiObject_Dispose.md) | (Унаследован от [UiObject](T_TFlex_Dialogs_UiObject.md)) |
|  | [Dispose(Boolean)](M_TFlex_Dialogs_BaseControl_Dispose.md) | (Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [EndCellEditing](M_TFlex_Dialogs_ListControl_EndCellEditing.md) |  |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ExpandAll](M_TFlex_Dialogs_ListControl_ExpandAll.md) | Развернуть все строки. IsHierarchyOn должно быть true. |
|  | [ExpandAllTheWayTo(Int32)](M_TFlex_Dialogs_ListControl_ExpandAllTheWayTo.md) | Развернуть все строки до row. IsHierarchyOn должно быть true. |
|  | [ExpandAllTheWayTo(Int64)](M_TFlex_Dialogs_ListControl_ExpandAllTheWayTo_1.md) | Развернуть все строки до строки с идентификатором rowId. IsHierarchyOn должно быть true. |
|  | [Finalize](M_TFlex_Dialogs_UiObject_Finalize.md) | (Унаследован от [UiObject](T_TFlex_Dialogs_UiObject.md)) |
|  | [Focus](M_TFlex_Dialogs_BaseControl_Focus.md) | Установить фокус ввода на элемент(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetRowById](M_TFlex_Dialogs_ListControl_GetRowById.md) | Получить идекс строки по идентификатору. IsIdMappingOn должно быть true. |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IsCellEditable](M_TFlex_Dialogs_ListControl_IsCellEditable.md) |  |
|  | [IsExpanded(Int32)](M_TFlex_Dialogs_ListControl_IsExpanded.md) | Развернута ли строка. |
|  | [IsExpanded(Int64)](M_TFlex_Dialogs_ListControl_IsExpanded_1.md) | Развернута ли строка. |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveAllEventHandlers](M_TFlex_Dialogs_BaseControl_RemoveAllEventHandlers.md) | Отписать все подписанные обработчики событий(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetCustomLocalizationId(String)](M_TFlex_Dialogs_BaseControl_SetCustomLocalizationId.md) | Задать отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetCustomLocalizationId(String, Boolean)](M_TFlex_Dialogs_BaseControl_SetCustomLocalizationId_1.md) | Задать отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetExpanded(Int32, Boolean)](M_TFlex_Dialogs_ListControl_SetExpanded.md) | Развернута ли строка. IsHierarchyOn должно быть true. |
|  | [SetExpanded(Int64, Boolean)](M_TFlex_Dialogs_ListControl_SetExpanded_1.md) | Развернута ли строка. IsHierarchyOn должно быть true. |
|  | [SuppressEvents](M_TFlex_Dialogs_BaseControl_SuppressEvents.md) | Заглушить события(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SuppressEvents(Boolean)](M_TFlex_Dialogs_BaseControl_SuppressEvents_1.md) | Заглушить события(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activated](E_TFlex_Dialogs_BaseControl_Activated.md) | Событие активации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ActiveChanged](E_TFlex_Dialogs_BaseControl_ActiveChanged.md) | Событие активации либо деактивации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [CellEditBegin](E_TFlex_Dialogs_ListControl_CellEditBegin.md) |  |
|  | [CellEditEnd](E_TFlex_Dialogs_ListControl_CellEditEnd.md) |  |
|  | [ContextMenuClicked](E_TFlex_Dialogs_ListControl_ContextMenuClicked.md) | Событие о нажатии в контекстном меню |
|  | [ContextMenuOpening](E_TFlex_Dialogs_ListControl_ContextMenuOpening.md) | Событие об открытии контекстного меню |
|  | [Deactivated](E_TFlex_Dialogs_BaseControl_Deactivated.md) | Событие деактивации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [FocusChanged](E_TFlex_Dialogs_BaseControl_FocusChanged.md) | Событие получения либо потери фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GotFocus](E_TFlex_Dialogs_BaseControl_GotFocus.md) | Событие получения фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IconClicked](E_TFlex_Dialogs_ListControl_IconClicked.md) | Событие при клике в иконку списка |
|  | [ItemExpandChanged](E_TFlex_Dialogs_ListControl_ItemExpandChanged.md) | Событие о смене развернутости элементов списка |
|  | [ItemHighlighted](E_TFlex_Dialogs_ListControl_ItemHighlighted.md) | Событие наведения указателя мыши на объект в списке |
|  | [Locked](E_TFlex_Dialogs_BaseControl_Locked.md) | Событие установки флажка у чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockedChanged](E_TFlex_Dialogs_BaseControl_LockedChanged.md) | Событие клика по чекбоксу метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LostFocus](E_TFlex_Dialogs_BaseControl_LostFocus.md) | Событие потери фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SelectionChanged](E_TFlex_Dialogs_ListControl_SelectionChanged.md) | Событие о смене выбранных элементов списка |
|  | [Unlocked](E_TFlex_Dialogs_BaseControl_Unlocked.md) | Событие снятия флажка у чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)

[SimpleListControl](T_TFlex_Dialogs_SimpleListControl.md)