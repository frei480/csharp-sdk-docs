

Руководство по T-FLEX CAD Open API

# ObjectSelectControl - класс  
  
---  
  
Элемент управления для выбора объектов. Показывается в виде поля ввода или списка.

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.DialogsUiObject](T_TFlex_Dialogs_UiObject.md) [TFlex.DialogsBaseControl](T_TFlex_Dialogs_BaseControl.md) TFlex.DialogsObjectSelectControl

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public class ObjectSelectControl : BaseControl
```
```vb
Public Class ObjectSelectControl
	Inherits BaseControl
```
```cpp
public ref class ObjectSelectControl : public BaseControl
```


Тип ObjectSelectControl предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ObjectSelectControl](M_TFlex_Dialogs_ObjectSelectControl__ctor.md) | Инициализирует новый экземпляр класса ObjectSelectControl |
|  | [ObjectSelectControl(String)](M_TFlex_Dialogs_ObjectSelectControl__ctor_1.md) | Инициализирует новый экземпляр класса ObjectSelectControl |
|  | [ObjectSelectControl(String, ObjectSelectControlMode)](M_TFlex_Dialogs_ObjectSelectControl__ctor_2.md) | Инициализирует новый экземпляр класса ObjectSelectControl |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AllowUserAdd](P_TFlex_Dialogs_ObjectSelectControl_AllowUserAdd.md) | Разрешает пользователю инициировать добавление новых объектов |
|  | [AllowUserClear](P_TFlex_Dialogs_ObjectSelectControl_AllowUserClear.md) | Разрешает пользователю очищать список |
|  | [AllowUserRemove](P_TFlex_Dialogs_ObjectSelectControl_AllowUserRemove.md) | Разрешает пользователю удаление объектов |
|  | [AutoAddLabelColon](P_TFlex_Dialogs_BaseControl_AutoAddLabelColon.md) | Автоматически добавлять двоеточие к метке(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [AutoBeginUserInsert](P_TFlex_Dialogs_ObjectSelectControl_AutoBeginUserInsert.md) | Постоянно находится в режиме добавления или редактирования объекта |
|  | [AutoEnableButtons](P_TFlex_Dialogs_ObjectSelectControl_AutoEnableButtons.md) | Автоматическое управление состоянием доступности кнопок |
|  | [AutoRequirementMet](P_TFlex_Dialogs_ObjectSelectControl_AutoRequirementMet.md) | Автоматически выставлять свойство IsRequarementMet. Также см. IsRequired. |
|  | [AutoSelectNextAfterRemove](P_TFlex_Dialogs_ObjectSelectControl_AutoSelectNextAfterRemove.md) | Выделять следующий объект после удаления |
|  | [Children](P_TFlex_Dialogs_BaseControl_Children.md) | Доступ к дочерним элементам(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [CustomLocalizationId](P_TFlex_Dialogs_BaseControl_CustomLocalizationId.md) | Отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ExtendedHintText](P_TFlex_Dialogs_BaseControl_ExtendedHintText.md) | Расширенный текст подсказки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Filter](P_TFlex_Dialogs_ObjectSelectControl_Filter.md) | Управление фильтром поиска |
|  | [FullId](P_TFlex_Dialogs_BaseControl_FullId.md) | Полный идентификатор элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HighlightedRow](P_TFlex_Dialogs_ObjectSelectControl_HighlightedRow.md) | Индекс объекта, над которым в списке находится указатель мыши |
|  | [HintDelay](P_TFlex_Dialogs_BaseControl_HintDelay.md) | Задержка показа подсказки в миллисекундах(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintDuration](P_TFlex_Dialogs_BaseControl_HintDuration.md) | Продолжительность показа подсказки в миллисекундах(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintIcon](P_TFlex_Dialogs_BaseControl_HintIcon.md) | Изображение для подсказки. Изображение показывается во всплывающей подсказке.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintText](P_TFlex_Dialogs_BaseControl_HintText.md) | Текст подсказки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HorizontalAlignment](P_TFlex_Dialogs_BaseControl_HorizontalAlignment.md) | Горизонтальное выравнивание элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Id](P_TFlex_Dialogs_BaseControl_Id.md) | Идентификатор элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IndexInParent](P_TFlex_Dialogs_BaseControl_IndexInParent.md) | Индекс в родительском элементе(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsActive](P_TFlex_Dialogs_BaseControl_IsActive.md) | Элемент является текущим активным элементом в форме(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsEnabled](P_TFlex_Dialogs_BaseControl_IsEnabled.md) | Элемент включён(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsFocused](P_TFlex_Dialogs_BaseControl_IsFocused.md) | Элемент имеет фокус ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsInUserEdit](P_TFlex_Dialogs_ObjectSelectControl_IsInUserEdit.md) | Возвращает true если элемент управления находится в режиме редактирования |
|  | [IsReadOnly](P_TFlex_Dialogs_BaseControl_IsReadOnly.md) | Элемент только для чтения(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRequired](P_TFlex_Dialogs_BaseControl_IsRequired.md) | Обязательный параметр. Влияет на отображение элемента.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRequirementMet](P_TFlex_Dialogs_BaseControl_IsRequirementMet.md) | Обязательный параметр заполнен. Связан со свойством IsRequired. Влияет на отображение элемента.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
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
|  | [Mode](P_TFlex_Dialogs_ObjectSelectControl_Mode.md) | Режим выбора объектов |
|  | [Objects](P_TFlex_Dialogs_ObjectSelectControl_Objects.md) | Доступ к объектам, отображаемым в списке |
|  | [Parent](P_TFlex_Dialogs_BaseControl_Parent.md) | Родительский элемент(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [PlaceholderText](P_TFlex_Dialogs_BaseControl_PlaceholderText.md) | Замещающий текст(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SelectedRow](P_TFlex_Dialogs_ObjectSelectControl_SelectedRow.md) | Возвращает первый выбранный объект или -1 |
|  | [SelectedRows](P_TFlex_Dialogs_ObjectSelectControl_SelectedRows.md) | Возвращает коллекцию индексов выбранных элементов |
|  | [SingleObject](P_TFlex_Dialogs_ObjectSelectControl_SingleObject.md) | Используется для установки или получения объекта, когда элемент управления находится в режиме выбора одного объекта |
|  | [StopEditOnActiveLost](P_TFlex_Dialogs_ObjectSelectControl_StopEditOnActiveLost.md) | Прекращать редактирование если элемент управления перестаёт быть активным |
|  | [Tag](P_TFlex_Dialogs_BaseControl_Tag.md) | Пользовательские данные(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [UserEditObject](P_TFlex_Dialogs_ObjectSelectControl_UserEditObject.md) | Получить или установить данные редактируемого объекта |
|  | [UserEditObjectItem](P_TFlex_Dialogs_ObjectSelectControl_UserEditObjectItem.md) | Возвращает редактируемый элемент |
|  | [UserEditPos](P_TFlex_Dialogs_ObjectSelectControl_UserEditPos.md) | Возвращает положение редактируемого элемента |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Dialogs_BaseControl_Activate.md) | Сделать элемент текущим активным элементом(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [BeginUserEdit](M_TFlex_Dialogs_ObjectSelectControl_BeginUserEdit.md) | Начать операцию пользовательского редактирования указанного объекта |
|  | [BeginUserInsert](M_TFlex_Dialogs_ObjectSelectControl_BeginUserInsert.md) | Начать операцию пользовательского добавления нового объекта |
|  | [BeginUserInsert(Int32)](M_TFlex_Dialogs_ObjectSelectControl_BeginUserInsert_1.md) | Начать операцию пользовательского добавления нового объекта |
|  | [DisableLocalization](M_TFlex_Dialogs_BaseControl_DisableLocalization.md) | Отключить локализацию данного элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Dispose](M_TFlex_Dialogs_UiObject_Dispose.md) | (Унаследован от [UiObject](T_TFlex_Dialogs_UiObject.md)) |
|  | [Dispose(Boolean)](M_TFlex_Dialogs_BaseControl_Dispose.md) | (Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [DoAutoEnableButtons](M_TFlex_Dialogs_ObjectSelectControl_DoAutoEnableButtons.md) | Выполнить включение или выключение кнопок согласно состоянию |
|  | [EndUserEdit](M_TFlex_Dialogs_ObjectSelectControl_EndUserEdit.md) | Завершить операцию пользовательского добавления/редактирования объектов |
|  | [EndUserEdit(ObjectSelectControlItem)](M_TFlex_Dialogs_ObjectSelectControl_EndUserEdit_1.md) | Завершить операцию пользовательского добавления/редактирования объектов |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Dialogs_UiObject_Finalize.md) | (Унаследован от [UiObject](T_TFlex_Dialogs_UiObject.md)) |
|  | [Focus](M_TFlex_Dialogs_BaseControl_Focus.md) | Установить фокус ввода на элемент(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveAllEventHandlers](M_TFlex_Dialogs_BaseControl_RemoveAllEventHandlers.md) | Отписать все подписанные обработчики событий(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [RemoveSelectedObjects](M_TFlex_Dialogs_ObjectSelectControl_RemoveSelectedObjects.md) | Удалить выбранные объекты |
|  | [RemoveSelectedObjects(Boolean)](M_TFlex_Dialogs_ObjectSelectControl_RemoveSelectedObjects_1.md) | Удалить выбранные объекты |
|  | [ResetFilter](M_TFlex_Dialogs_ObjectSelectControl_ResetFilter.md) | Сбрасывает фильтр поиска |
|  | [SetAutoBeginUserInsert(Boolean)](M_TFlex_Dialogs_ObjectSelectControl_SetAutoBeginUserInsert.md) | Постоянно находится в режиме добавления или редактирования объекта |
|  | [SetAutoBeginUserInsert(Boolean, Boolean)](M_TFlex_Dialogs_ObjectSelectControl_SetAutoBeginUserInsert_1.md) | Постоянно находится в режиме добавления или редактирования объекта |
|  | [SetCustomLocalizationId(String)](M_TFlex_Dialogs_BaseControl_SetCustomLocalizationId.md) | Задать отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetCustomLocalizationId(String, Boolean)](M_TFlex_Dialogs_BaseControl_SetCustomLocalizationId_1.md) | Задать отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetFilter(ObjectSelectControlFilter)](M_TFlex_Dialogs_ObjectSelectControl_SetFilter_1.md) | Устанавливает фильтр поиска |
|  | [SetFilter(FuncObjectSelectControlPlainObject, Boolean, Document)](M_TFlex_Dialogs_ObjectSelectControl_SetFilter.md) |  |
|  | [SetSingleObject(ModelObject)](M_TFlex_Dialogs_ObjectSelectControl_SetSingleObject_2.md) | Устанавливает объект, когда элемент управления находится в режиме выбора одного объекта |
|  | [SetSingleObject(ObjectSelectControlPlainObject)](M_TFlex_Dialogs_ObjectSelectControl_SetSingleObject.md) | Устанавливает объект, когда элемент управления находится в режиме выбора одного объекта |
|  | [SetSingleObject(ModelObject, Boolean)](M_TFlex_Dialogs_ObjectSelectControl_SetSingleObject_3.md) | Устанавливает объект, когда элемент управления находится в режиме выбора одного объекта |
|  | [SetSingleObject(ObjectSelectControlPlainObject, Boolean)](M_TFlex_Dialogs_ObjectSelectControl_SetSingleObject_1.md) | Устанавливает объект, когда элемент управления находится в режиме выбора одного объекта |
|  | [SuppressEvents](M_TFlex_Dialogs_BaseControl_SuppressEvents.md) | Заглушить события(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SuppressEvents(Boolean)](M_TFlex_Dialogs_BaseControl_SuppressEvents_1.md) | Заглушить события(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activated](E_TFlex_Dialogs_BaseControl_Activated.md) | Событие активации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ActiveChanged](E_TFlex_Dialogs_BaseControl_ActiveChanged.md) | Событие активации либо деактивации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Deactivated](E_TFlex_Dialogs_BaseControl_Deactivated.md) | Событие деактивации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [FocusChanged](E_TFlex_Dialogs_BaseControl_FocusChanged.md) | Событие получения либо потери фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GotFocus](E_TFlex_Dialogs_BaseControl_GotFocus.md) | Событие получения фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ItemHighlighted](E_TFlex_Dialogs_ObjectSelectControl_ItemHighlighted.md) | Событие наведения указателя мыши на объект в списке |
|  | [Locked](E_TFlex_Dialogs_BaseControl_Locked.md) | Событие установки флажка у чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockedChanged](E_TFlex_Dialogs_BaseControl_LockedChanged.md) | Событие клика по чекбоксу метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LostFocus](E_TFlex_Dialogs_BaseControl_LostFocus.md) | Событие потери фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ObjectReplacedByUser](E_TFlex_Dialogs_ObjectSelectControl_ObjectReplacedByUser.md) | Событие замены объекта пользователем |
|  | [StateUpdated](E_TFlex_Dialogs_ObjectSelectControl_StateUpdated.md) | Событие изменения состояния |
|  | [Unlocked](E_TFlex_Dialogs_BaseControl_Unlocked.md) | Событие снятия флажка у чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)