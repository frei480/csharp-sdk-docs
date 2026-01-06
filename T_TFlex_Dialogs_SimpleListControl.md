

Руководство по T-FLEX CAD Open API

# SimpleListControl - класс  
    
Упрощённый вариант ListControl, позволяющий избежать явного создания класса модели данных для простых списков

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.DialogsUiObject](T_TFlex_Dialogs_UiObject.md) [TFlex.DialogsBaseControl](T_TFlex_Dialogs_BaseControl.md) [TFlex.DialogsListControl](T_TFlex_Dialogs_ListControl.md) TFlex.DialogsSimpleListControl

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public class SimpleListControl : ListControl
```
```vb
Public Class SimpleListControl
	Inherits ListControl
```
```cpp
public ref class SimpleListControl : public ListControl
```


Тип SimpleListControl предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [SimpleListControl](M_TFlex_Dialogs_SimpleListControl__ctor.md) | Инициализирует новый экземпляр класса SimpleListControl |
|  | [SimpleListControl(String)](M_TFlex_Dialogs_SimpleListControl__ctor_1.md) | Инициализирует новый экземпляр класса SimpleListControl |
|  | [SimpleListControl(String, Int32)](M_TFlex_Dialogs_SimpleListControl__ctor_2.md) | Инициализирует новый экземпляр класса SimpleListControl |
|  | [SimpleListControl(String, Int32, Int32)](M_TFlex_Dialogs_SimpleListControl__ctor_3.md) | Инициализирует новый экземпляр класса SimpleListControl |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AutoAddLabelColon](P_TFlex_Dialogs_BaseControl_AutoAddLabelColon.md) | Автоматически добавлять двоеточие к метке(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Buttons](P_TFlex_Dialogs_ListControl_Buttons.md) | Коллекция кнопок, отображаемых контролом(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Children](P_TFlex_Dialogs_BaseControl_Children.md) | Доступ к дочерним элементам(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ColumnCount](P_TFlex_Dialogs_SimpleListControl_ColumnCount.md) | Количество столбцов в списке |
|  | [CustomLocalizationId](P_TFlex_Dialogs_BaseControl_CustomLocalizationId.md) | Отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [EditingCell](P_TFlex_Dialogs_ListControl_EditingCell.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [EditMode](P_TFlex_Dialogs_ListControl_EditMode.md) | Режим редактирования ячеек ListControl-а(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Editors](P_TFlex_Dialogs_ListControl_Editors.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [ExtendedHintText](P_TFlex_Dialogs_BaseControl_ExtendedHintText.md) | Расширенный текст подсказки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [FullId](P_TFlex_Dialogs_BaseControl_FullId.md) | Полный идентификатор элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GridLinesVisibility](P_TFlex_Dialogs_ListControl_GridLinesVisibility.md) | Режим отображения линий сетки(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [HintDelay](P_TFlex_Dialogs_BaseControl_HintDelay.md) | Задержка показа подсказки в миллисекундах(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintDuration](P_TFlex_Dialogs_BaseControl_HintDuration.md) | Продолжительность показа подсказки в миллисекундах(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintIcon](P_TFlex_Dialogs_BaseControl_HintIcon.md) | Изображение для подсказки. Изображение показывается во всплывающей подсказке.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintText](P_TFlex_Dialogs_BaseControl_HintText.md) | Текст подсказки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HorizontalAlignment](P_TFlex_Dialogs_BaseControl_HorizontalAlignment.md) | Горизонтальное выравнивание элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Id](P_TFlex_Dialogs_BaseControl_Id.md) | Идентификатор элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IndexInParent](P_TFlex_Dialogs_BaseControl_IndexInParent.md) | Индекс в родительском элементе(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsActive](P_TFlex_Dialogs_BaseControl_IsActive.md) | Элемент является текущим активным элементом в форме(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsEditingCell](P_TFlex_Dialogs_ListControl_IsEditingCell.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [IsEnabled](P_TFlex_Dialogs_BaseControl_IsEnabled.md) | Элемент включён(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsFocused](P_TFlex_Dialogs_BaseControl_IsFocused.md) | Элемент имеет фокус ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsHierarchyOn](P_TFlex_Dialogs_ListControl_IsHierarchyOn.md) | Включить поддержку иерархии строк. Для задания вложенность задается родительская строка.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [IsIdMappingOn](P_TFlex_Dialogs_ListControl_IsIdMappingOn.md) | Включить поддержку идентификации строк по id(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [IsReadOnly](P_TFlex_Dialogs_BaseControl_IsReadOnly.md) | Элемент только для чтения(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRequired](P_TFlex_Dialogs_BaseControl_IsRequired.md) | Обязательный параметр. Влияет на отображение элемента.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRequirementMet](P_TFlex_Dialogs_BaseControl_IsRequirementMet.md) | Обязательный параметр заполнен. Связан со свойством IsRequired. Влияет на отображение элемента.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsStretchHeight](P_TFlex_Dialogs_ListControl_IsStretchHeight.md) | Элемент управления растянут по вертикали, чтобы заполнить все доступное пространство.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
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
|  | [Model](P_TFlex_Dialogs_ListControl_Model.md) | Модель данных списка(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Parent](P_TFlex_Dialogs_BaseControl_Parent.md) | Родительский элемент(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [PlaceholderText](P_TFlex_Dialogs_BaseControl_PlaceholderText.md) | Замещающий текст(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [RowCount](P_TFlex_Dialogs_SimpleListControl_RowCount.md) | Количество строк в списке |
|  | [SelectedRow](P_TFlex_Dialogs_ListControl_SelectedRow.md) | Возвращает индекс первой выбранной строки или -1(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [SelectedRows](P_TFlex_Dialogs_ListControl_SelectedRows.md) | Коллекция индексов выбранных элементов(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Tag](P_TFlex_Dialogs_BaseControl_Tag.md) | Пользовательские данные(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Dialogs_BaseControl_Activate.md) | Сделать элемент текущим активным элементом(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [AddRow](M_TFlex_Dialogs_SimpleListControl_AddRow.md) | Вставить строку в конец списка |
|  | [AddRow(IList)](M_TFlex_Dialogs_SimpleListControl_AddRow_1.md) | Вставить строку в конец списка |
|  | [AddRow(Object)](M_TFlex_Dialogs_SimpleListControl_AddRow_2.md) | Вставить строку в конец списка |
|  | [AddRow(Object)](M_TFlex_Dialogs_SimpleListControl_AddRow_3.md) | Вставить строку в конец списка |
|  | [AddRows](M_TFlex_Dialogs_SimpleListControl_AddRows.md) | Вставить строки в конец списка |
|  | [BeginCellEditing(CellInfo)](M_TFlex_Dialogs_ListControl_BeginCellEditing_1.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [BeginCellEditing(Int32, Int32)](M_TFlex_Dialogs_ListControl_BeginCellEditing.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [CollapseAll](M_TFlex_Dialogs_ListControl_CollapseAll.md) | Свернуть все строки. IsHierarchyOn должно быть true.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [DisableLocalization](M_TFlex_Dialogs_BaseControl_DisableLocalization.md) | Отключить локализацию данного элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Dispose](M_TFlex_Dialogs_UiObject_Dispose.md) | (Унаследован от [UiObject](T_TFlex_Dialogs_UiObject.md)) |
|  | [Dispose(Boolean)](M_TFlex_Dialogs_BaseControl_Dispose.md) | (Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [EndCellEditing](M_TFlex_Dialogs_ListControl_EndCellEditing.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ExpandAll](M_TFlex_Dialogs_ListControl_ExpandAll.md) | Развернуть все строки. IsHierarchyOn должно быть true.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [ExpandAllTheWayTo(Int32)](M_TFlex_Dialogs_ListControl_ExpandAllTheWayTo.md) | Развернуть все строки до row. IsHierarchyOn должно быть true.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [ExpandAllTheWayTo(Int64)](M_TFlex_Dialogs_ListControl_ExpandAllTheWayTo_1.md) | Развернуть все строки до строки с идентификатором rowId. IsHierarchyOn должно быть true.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Finalize](M_TFlex_Dialogs_UiObject_Finalize.md) | (Унаследован от [UiObject](T_TFlex_Dialogs_UiObject.md)) |
|  | [Focus](M_TFlex_Dialogs_BaseControl_Focus.md) | Установить фокус ввода на элемент(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GetAlignment](M_TFlex_Dialogs_SimpleListControl_GetAlignment.md) | Возвращает выравние для ячейки |
|  | [GetCheckState](M_TFlex_Dialogs_SimpleListControl_GetCheckState.md) | Возвращает CheckState элемента списка |
|  | [GetContent](M_TFlex_Dialogs_SimpleListControl_GetContent.md) | Возвращает содержимое ячейки списка |
|  | [GetDefaultAlignment](M_TFlex_Dialogs_SimpleListControl_GetDefaultAlignment.md) | Возвращает выравние по умолчанию для колонки |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHeader](M_TFlex_Dialogs_SimpleListControl_GetHeader.md) | Возвращает данные заголовка списка |
|  | [GetIcon](M_TFlex_Dialogs_SimpleListControl_GetIcon.md) | Возвращает иконку элемента списка |
|  | [GetParentRow](M_TFlex_Dialogs_SimpleListControl_GetParentRow.md) | Получить индекс родительской строки. Должен быть включен режим IsHierarchyOn. |
|  | [GetRowById](M_TFlex_Dialogs_ListControl_GetRowById.md) | Получить идекс строки по идентификатору. IsIdMappingOn должно быть true.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [GetRowId](M_TFlex_Dialogs_SimpleListControl_GetRowId.md) | Получить идентификатор строки. Должен быть включен режим IsIdMappingOn. |
|  | [GetToolTip](M_TFlex_Dialogs_SimpleListControl_GetToolTip.md) | Возвращает подсказку элемента списка |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetWidthCoefficient](M_TFlex_Dialogs_SimpleListControl_GetWidthCoefficient.md) | Возвращает коэффициент ширины столбца |
|  | [HasAlignment](M_TFlex_Dialogs_SimpleListControl_HasAlignment.md) | Возвращает true, если выставлено выравние для ячейки |
|  | [HasDefaultAlignment](M_TFlex_Dialogs_SimpleListControl_HasDefaultAlignment.md) | Возвращает true, если выставлено выравние по умолчанию для колонки |
|  | [InsertRow(Int32)](M_TFlex_Dialogs_SimpleListControl_InsertRow.md) | Вставить строку в список |
|  | [InsertRow(Int32, IList)](M_TFlex_Dialogs_SimpleListControl_InsertRow_1.md) | Вставить строку в список |
|  | [InsertRow(Int32, Object)](M_TFlex_Dialogs_SimpleListControl_InsertRow_2.md) | Вставить строку в список |
|  | [InsertRow(Int32, Object)](M_TFlex_Dialogs_SimpleListControl_InsertRow_3.md) | Вставить строку в список |
|  | [InsertRows](M_TFlex_Dialogs_SimpleListControl_InsertRows.md) | Вставить строки в список |
|  | [IsCellEditable(CellInfo)](M_TFlex_Dialogs_ListControl_IsCellEditable.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [IsCellEditable(Int32, Int32)](M_TFlex_Dialogs_SimpleListControl_IsCellEditable.md) |  |
|  | [IsCellEditableSet](M_TFlex_Dialogs_SimpleListControl_IsCellEditableSet.md) |  |
|  | [IsColumnEditable](M_TFlex_Dialogs_SimpleListControl_IsColumnEditable.md) |  |
|  | [IsColumnEditableSet](M_TFlex_Dialogs_SimpleListControl_IsColumnEditableSet.md) |  |
|  | [IsColumnTree](M_TFlex_Dialogs_SimpleListControl_IsColumnTree.md) | Колонка для отображения структуры дерева |
|  | [IsExpanded(Int32)](M_TFlex_Dialogs_ListControl_IsExpanded.md) | Развернута ли строка.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [IsExpanded(Int64)](M_TFlex_Dialogs_ListControl_IsExpanded_1.md) | Развернута ли строка.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveAll](M_TFlex_Dialogs_SimpleListControl_RemoveAll.md) | Удалить все строки из списка |
|  | [RemoveAllEventHandlers](M_TFlex_Dialogs_BaseControl_RemoveAllEventHandlers.md) | Отписать все подписанные обработчики событий(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [RemoveRow](M_TFlex_Dialogs_SimpleListControl_RemoveRow.md) | Удалить строку из списка |
|  | [RemoveRows](M_TFlex_Dialogs_SimpleListControl_RemoveRows.md) | Удалить строки из списка |
|  | [SetAlignment](M_TFlex_Dialogs_SimpleListControl_SetAlignment.md) |  |
|  | [SetCellEditable](M_TFlex_Dialogs_SimpleListControl_SetCellEditable.md) |  |
|  | [SetCheckState](M_TFlex_Dialogs_SimpleListControl_SetCheckState.md) |  |
|  | [SetColumnEditable](M_TFlex_Dialogs_SimpleListControl_SetColumnEditable.md) |  |
|  | [SetColumnGroup](M_TFlex_Dialogs_SimpleListControl_SetColumnGroup.md) |  |
|  | [SetColumnTree](M_TFlex_Dialogs_SimpleListControl_SetColumnTree.md) | Колонка для отображения структуры дерева |
|  | [SetContent](M_TFlex_Dialogs_SimpleListControl_SetContent.md) | Устанавливает содержимое ячейки списка |
|  | [SetCustomLocalizationId(String)](M_TFlex_Dialogs_BaseControl_SetCustomLocalizationId.md) | Задать отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetCustomLocalizationId(String, Boolean)](M_TFlex_Dialogs_BaseControl_SetCustomLocalizationId_1.md) | Задать отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetDefaultAlignment](M_TFlex_Dialogs_SimpleListControl_SetDefaultAlignment.md) |  |
|  | [SetExpanded(Int32, Boolean)](M_TFlex_Dialogs_ListControl_SetExpanded.md) | Развернута ли строка. IsHierarchyOn должно быть true.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [SetExpanded(Int64, Boolean)](M_TFlex_Dialogs_ListControl_SetExpanded_1.md) | Развернута ли строка. IsHierarchyOn должно быть true.(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [SetHeader(Object)](M_TFlex_Dialogs_SimpleListControl_SetHeader_1.md) | Устанавливает данные заголовка списка |
|  | [SetHeader(Int32, Object)](M_TFlex_Dialogs_SimpleListControl_SetHeader.md) | Устанавливает данные заголовка списка |
|  | [SetHeaderIcon](M_TFlex_Dialogs_SimpleListControl_SetHeaderIcon.md) | Устанавливает иконку для заголовка колонки |
|  | [SetHeaders(IList)](M_TFlex_Dialogs_SimpleListControl_SetHeaders.md) | Устанавливает данные всех заголовков списка |
|  | [SetHeaders(Object)](M_TFlex_Dialogs_SimpleListControl_SetHeaders_1.md) | Устанавливает данные всех заголовков списка |
|  | [SetHeaderToolTip](M_TFlex_Dialogs_SimpleListControl_SetHeaderToolTip.md) | Устанавливает подсказку для заголовка колонки |
|  | [SetIcon](M_TFlex_Dialogs_SimpleListControl_SetIcon.md) | Устанавливает иконку элемента списка |
|  | [SetParentRow](M_TFlex_Dialogs_SimpleListControl_SetParentRow.md) | Установить индекс родительской строки. Должен быть включен режим IsHierarchyOn. |
|  | [SetParentRowId](M_TFlex_Dialogs_SimpleListControl_SetParentRowId.md) | Установить индекс родительской строки. Должены быть включены режим IsHierarchyOn и IsIdMappingOn. |
|  | [SetRowContent(Int32, IList)](M_TFlex_Dialogs_SimpleListControl_SetRowContent.md) | Устанавливает содержимое ячеек в строке списка |
|  | [SetRowContent(Int32, Object)](M_TFlex_Dialogs_SimpleListControl_SetRowContent_1.md) | Устанавливает содержимое ячеек в строке списка |
|  | [SetRowContent(Int32, Object)](M_TFlex_Dialogs_SimpleListControl_SetRowContent_2.md) | Устанавливает содержимое ячеек в строке списка |
|  | [SetRowId](M_TFlex_Dialogs_SimpleListControl_SetRowId.md) | Установить идентификатор строки. Должен быть включен режим IsIdMappingOn. |
|  | [SetToolTip](M_TFlex_Dialogs_SimpleListControl_SetToolTip.md) | Устанавливает подсказку элемента списка |
|  | [SetWidthCoefficient](M_TFlex_Dialogs_SimpleListControl_SetWidthCoefficient.md) | Устанавливает коэффициент ширины столбца |
|  | [SetWidthCoefficients(Double)](M_TFlex_Dialogs_SimpleListControl_SetWidthCoefficients_1.md) | Устанавливает коэффициенты ширины всех столбцов |
|  | [SetWidthCoefficients(IListDouble)](M_TFlex_Dialogs_SimpleListControl_SetWidthCoefficients.md) |  |
|  | [SuppressEvents](M_TFlex_Dialogs_BaseControl_SuppressEvents.md) | Заглушить события(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SuppressEvents(Boolean)](M_TFlex_Dialogs_BaseControl_SuppressEvents_1.md) | Заглушить события(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activated](E_TFlex_Dialogs_BaseControl_Activated.md) | Событие активации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ActiveChanged](E_TFlex_Dialogs_BaseControl_ActiveChanged.md) | Событие активации либо деактивации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [CellEditBegin](E_TFlex_Dialogs_ListControl_CellEditBegin.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [CellEditEnd](E_TFlex_Dialogs_ListControl_CellEditEnd.md) | (Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [CheckStateChanged](E_TFlex_Dialogs_SimpleListControl_CheckStateChanged.md) | Событие смены значения чекбокса |
|  | [ContextMenuClicked](E_TFlex_Dialogs_ListControl_ContextMenuClicked.md) | Событие о нажатии в контекстном меню(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [ContextMenuOpening](E_TFlex_Dialogs_ListControl_ContextMenuOpening.md) | Событие об открытии контекстного меню(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Deactivated](E_TFlex_Dialogs_BaseControl_Deactivated.md) | Событие деактивации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [FocusChanged](E_TFlex_Dialogs_BaseControl_FocusChanged.md) | Событие получения либо потери фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GotFocus](E_TFlex_Dialogs_BaseControl_GotFocus.md) | Событие получения фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IconClicked](E_TFlex_Dialogs_ListControl_IconClicked.md) | Событие при клике в иконку списка(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [ItemExpandChanged](E_TFlex_Dialogs_ListControl_ItemExpandChanged.md) | Событие о смене развернутости элементов списка(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [ItemHighlighted](E_TFlex_Dialogs_ListControl_ItemHighlighted.md) | Событие наведения указателя мыши на объект в списке(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Locked](E_TFlex_Dialogs_BaseControl_Locked.md) | Событие установки флажка у чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockedChanged](E_TFlex_Dialogs_BaseControl_LockedChanged.md) | Событие клика по чекбоксу метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LostFocus](E_TFlex_Dialogs_BaseControl_LostFocus.md) | Событие потери фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SelectionChanged](E_TFlex_Dialogs_ListControl_SelectionChanged.md) | Событие о смене выбранных элементов списка(Унаследован от [ListControl](T_TFlex_Dialogs_ListControl.md)) |
|  | [Unlocked](E_TFlex_Dialogs_BaseControl_Unlocked.md) | Событие снятия флажка у чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)