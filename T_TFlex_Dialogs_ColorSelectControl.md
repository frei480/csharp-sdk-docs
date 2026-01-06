

Руководство по T-FLEX CAD Open API

# ColorSelectControl - класс  
    
Контрол выбора цвета

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.DialogsUiObject](T_TFlex_Dialogs_UiObject.md) [TFlex.DialogsBaseControl](T_TFlex_Dialogs_BaseControl.md) [TFlex.DialogsInputControlBase](T_TFlex_Dialogs_InputControlBase.md) [TFlex.DialogsNumericInputControl](T_TFlex_Dialogs_NumericInputControl.md) TFlex.DialogsColorSelectControl

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public class ColorSelectControl : NumericInputControl
```




Тип ColorSelectControl предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ColorSelectControl](M_TFlex_Dialogs_ColorSelectControl__ctor.md) | Инициализирует новый экземпляр класса ColorSelectControl |
|  | [ColorSelectControl(String)](M_TFlex_Dialogs_ColorSelectControl__ctor_1.md) | Инициализирует новый экземпляр класса ColorSelectControl |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AllowVariable](P_TFlex_Dialogs_NumericInputControl_AllowVariable.md) | Управление флагом, разрешающим задание переменной пользователем(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [AutoAddLabelColon](P_TFlex_Dialogs_BaseControl_AutoAddLabelColon.md) | Автоматически добавлять двоеточие к метке(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [AutoApplyByTimeout](P_TFlex_Dialogs_NumericInputControl_AutoApplyByTimeout.md) | Управление флагом автоматического применения значения по таймауту. Имеет смысл когда пользователь вводит число, а не выражение.(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Buttons](P_TFlex_Dialogs_InputControlBase_Buttons.md) | Доступ к дополнительным кнопкам(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [CanDecrement](P_TFlex_Dialogs_NumericInputControl_CanDecrement.md) | Возвращает true, если можно уменьшить значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [CanIncrement](P_TFlex_Dialogs_NumericInputControl_CanIncrement.md) | Возвращает true, если можно увеличить значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Children](P_TFlex_Dialogs_BaseControl_Children.md) | Доступ к дочерним элементам(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ClampedValue](P_TFlex_Dialogs_NumericInputControl_ClampedValue.md) | Возвращает текущее значение, при необходимости обрезанное диапазоном допустимых значений (Range)(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [CurrentValueListIndex](P_TFlex_Dialogs_InputControlBase_CurrentValueListIndex.md) | Индекс текущего элемента списка (для итерации колёсиком мыши)(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [CustomLocalizationId](P_TFlex_Dialogs_BaseControl_CustomLocalizationId.md) | Отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [DefaultText](P_TFlex_Dialogs_NumericInputControl_DefaultText.md) | Возвращает значение по умолчанию в виде текста(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [DefaultUnit](P_TFlex_Dialogs_NumericInputControl_DefaultUnit.md) | Управление единицей измерения по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [DefaultValue](P_TFlex_Dialogs_NumericInputControl_DefaultValue.md) | Управление значением по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [DefaultVariable](P_TFlex_Dialogs_NumericInputControl_DefaultVariable.md) | Управление переменой по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [DefaultVariableStringValue](P_TFlex_Dialogs_NumericInputControl_DefaultVariableStringValue.md) | Возвращает значение переменной по умолчанию в виде текста(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [EffectiveIncrementStep](P_TFlex_Dialogs_NumericInputControl_EffectiveIncrementStep.md) | Реальный шаг прокрутки(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [EffectiveUserIncrementStep](P_TFlex_Dialogs_NumericInputControl_EffectiveUserIncrementStep.md) | Возвращает обработанный UserIncrementStep(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [ExtendedHintText](P_TFlex_Dialogs_BaseControl_ExtendedHintText.md) | Расширенный текст подсказки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [FocusLostBehavior](P_TFlex_Dialogs_InputControlBase_FocusLostBehavior.md) | Поведение при потере фокуса(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [FullId](P_TFlex_Dialogs_BaseControl_FullId.md) | Полный идентификатор элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HasDefaultValue](P_TFlex_Dialogs_NumericInputControl_HasDefaultValue.md) | Возвращает true, если значение по умолчанию задано(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [HasUpDown](P_TFlex_Dialogs_NumericInputControl_HasUpDown.md) | Показывать кнопки Up/Down(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [HasValue](P_TFlex_Dialogs_NumericInputControl_HasValue.md) | Возвращает True, если числовое значение доступно(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [HintDelay](P_TFlex_Dialogs_BaseControl_HintDelay.md) | Задержка показа подсказки в миллисекундах(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintDuration](P_TFlex_Dialogs_BaseControl_HintDuration.md) | Продолжительность показа подсказки в миллисекундах(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintIcon](P_TFlex_Dialogs_BaseControl_HintIcon.md) | Изображение для подсказки. Изображение показывается во всплывающей подсказке.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HintText](P_TFlex_Dialogs_BaseControl_HintText.md) | Текст подсказки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [HorizontalAlignment](P_TFlex_Dialogs_BaseControl_HorizontalAlignment.md) | Горизонтальное выравнивание элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Id](P_TFlex_Dialogs_BaseControl_Id.md) | Идентификатор элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IncrementStep](P_TFlex_Dialogs_NumericInputControl_IncrementStep.md) | Шаг прокрутки(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [IndexInParent](P_TFlex_Dialogs_BaseControl_IndexInParent.md) | Индекс в родительском элементе(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsActive](P_TFlex_Dialogs_BaseControl_IsActive.md) | Элемент является текущим активным элементом в форме(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsAutocomplete](P_TFlex_Dialogs_InputControlBase_IsAutocomplete.md) | Флаг индикатор того, что у контрола включено автодополнение(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [IsAutoFormat](P_TFlex_Dialogs_NumericInputControl_IsAutoFormat.md) | Управление флагом автоматического форматирования(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [IsDefaultValue](P_TFlex_Dialogs_NumericInputControl_IsDefaultValue.md) | Возвращает true, если текущее значение является значением по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [IsDirty](P_TFlex_Dialogs_InputControlBase_IsDirty.md) | Получить флаг IsDirty(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [IsEnabled](P_TFlex_Dialogs_BaseControl_IsEnabled.md) | Элемент включён(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsFocused](P_TFlex_Dialogs_BaseControl_IsFocused.md) | Элемент имеет фокус ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsIntegral](P_TFlex_Dialogs_NumericInputControl_IsIntegral.md) | Разрешать только целые числа(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [IsManyValues](P_TFlex_Dialogs_InputControlBase_IsManyValues.md) | Флаг индикатор того, что контрол отображает сразу несколько значений(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [IsReadOnly](P_TFlex_Dialogs_BaseControl_IsReadOnly.md) | Элемент только для чтения(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRequired](P_TFlex_Dialogs_BaseControl_IsRequired.md) | Обязательный параметр. Влияет на отображение элемента.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRequirementMet](P_TFlex_Dialogs_BaseControl_IsRequirementMet.md) | Обязательный параметр заполнен. Связан со свойством IsRequired. Влияет на отображение элемента.(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [IsRgbUsed](P_TFlex_Dialogs_ColorSelectControl_IsRgbUsed.md) | Использовать RGB вместо системных цветов T-FLEX CAD |
|  | [IsUserValue](P_TFlex_Dialogs_InputControlBase_IsUserValue.md) | Возвращает True, если текущее значение получено от пользователя(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [IsValid](P_TFlex_Dialogs_InputControlBase_IsValid.md) | Управление состоянием корректности ввода(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [IsValueInRange](P_TFlex_Dialogs_NumericInputControl_IsValueInRange.md) | Возвращает True, если числовое значение находится в пределах диапазоа допустимых значений (Range)(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [IsVisible](P_TFlex_Dialogs_BaseControl_IsVisible.md) | Элемент видимый(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Label](P_TFlex_Dialogs_BaseControl_Label.md) | Текст метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LabelPadding](P_TFlex_Dialogs_BaseControl_LabelPadding.md) | Выравнивание элемента по меткам(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LabelPosition](P_TFlex_Dialogs_BaseControl_LabelPosition.md) | Положение метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LocalizationMode](P_TFlex_Dialogs_BaseControl_LocalizationMode.md) | Режим локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockBehavior](P_TFlex_Dialogs_BaseControl_LockBehavior.md) | Режим работы чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockMode](P_TFlex_Dialogs_BaseControl_LockMode.md) | Режим отображения чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockPadding](P_TFlex_Dialogs_BaseControl_LockPadding.md) | Выравнивание меток по чекбоксам(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockState](P_TFlex_Dialogs_BaseControl_LockState.md) | Текущее значение чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ManyValuesText](P_TFlex_Dialogs_InputControlBase_ManyValuesText.md) | Текст, показываемый пользователю в режиме IsManyValues(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [Max](P_TFlex_Dialogs_NumericInputControl_Max.md) | Управление максимальным допустимым значением(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [MaxHeight](P_TFlex_Dialogs_BaseControl_MaxHeight.md) | Максимальная высота элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [MaxWidth](P_TFlex_Dialogs_BaseControl_MaxWidth.md) | Максимальная ширина элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Min](P_TFlex_Dialogs_NumericInputControl_Min.md) | Управление минимальным допустимым значением(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [MinHeight](P_TFlex_Dialogs_BaseControl_MinHeight.md) | Минимальная высота элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [MinWidth](P_TFlex_Dialogs_BaseControl_MinWidth.md) | Минимальная ширина элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [OriginalIsDefaultValue](P_TFlex_Dialogs_NumericInputControl_OriginalIsDefaultValue.md) | Возвращает True, если исходное (стабильное) значение является значением по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [OriginalUnit](P_TFlex_Dialogs_NumericInputControl_OriginalUnit.md) | Исходная (стабильная) единица измерения(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [OriginalValue](P_TFlex_Dialogs_NumericInputControl_OriginalValue.md) | Исходное (стабильное) значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [OriginalValueIsFromUser](P_TFlex_Dialogs_InputControlBase_OriginalValueIsFromUser.md) | Возвращает True, если стабильное значение получено от пользователя (а не задано программно)(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [OriginalVariable](P_TFlex_Dialogs_NumericInputControl_OriginalVariable.md) | Исходная (стабильная) переменная(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Parent](P_TFlex_Dialogs_BaseControl_Parent.md) | Родительский элемент(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [PlaceholderText](P_TFlex_Dialogs_BaseControl_PlaceholderText.md) | Замещающий текст(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Precision](P_TFlex_Dialogs_NumericInputControl_Precision.md) | Точность(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Range](P_TFlex_Dialogs_NumericInputControl_Range.md) | Управление диапазоном допустимых значений(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SelectionLength](P_TFlex_Dialogs_InputControlBase_SelectionLength.md) | Длина селекции(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [SelectionStart](P_TFlex_Dialogs_InputControlBase_SelectionStart.md) | Позиция начала селекции(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [SpinStepAction](P_TFlex_Dialogs_NumericInputControl_SpinStepAction.md) | Действие при прокрутке колёсиком мыши(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [State](P_TFlex_Dialogs_NumericInputControl_State.md) | Возвращает состояние NumericInputControl(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Tag](P_TFlex_Dialogs_BaseControl_Tag.md) | Пользовательские данные(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Text](P_TFlex_Dialogs_InputControlBase_Text.md) | Получить текст(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [Unit](P_TFlex_Dialogs_NumericInputControl_Unit.md) | Единица измерения(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [UserIncrementStep](P_TFlex_Dialogs_NumericInputControl_UserIncrementStep.md) | Шаг прокрутки, который может быть изменён пользователем(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Value](P_TFlex_Dialogs_NumericInputControl_Value.md) | Текущее значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [ValueList](P_TFlex_Dialogs_InputControlBase_ValueList.md) | Доступ к списку значений(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [ValueListMode](P_TFlex_Dialogs_InputControlBase_ValueListMode.md) | Режим списка значений(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [Variable](P_TFlex_Dialogs_NumericInputControl_Variable.md) | Текущая переменная(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [VariableStringValue](P_TFlex_Dialogs_NumericInputControl_VariableStringValue.md) | Возвращает значение текущей переменной как строку(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Dialogs_BaseControl_Activate.md) | Сделать элемент текущим активным элементом(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ApplyChanges](M_TFlex_Dialogs_InputControlBase_ApplyChanges.md) | Применить изменения пользователя(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [CanUserIncrement](M_TFlex_Dialogs_NumericInputControl_CanUserIncrement.md) | Возвращает true, если значение еще можно увеличить (уменьшить) без выхода за границы(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [ClearDefaultValue](M_TFlex_Dialogs_NumericInputControl_ClearDefaultValue.md) | Сбрасывает значение по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [ClearOriginalValueIsFromUser](M_TFlex_Dialogs_InputControlBase_ClearOriginalValueIsFromUser.md) | Сбрасывает значение флага OriginalValueIsFromUser(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [ClearValue](M_TFlex_Dialogs_NumericInputControl_ClearValue.md) | Сбросить текущее значение. Элемент будет отображать значение по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Decrement](M_TFlex_Dialogs_NumericInputControl_Decrement.md) | Уменьшить текущее значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Decrement(Boolean)](M_TFlex_Dialogs_NumericInputControl_Decrement_1.md) | Уменьшить текущее значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [DeselectAll](M_TFlex_Dialogs_InputControlBase_DeselectAll.md) | Сбросить селекцию текста(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [DisableLocalization](M_TFlex_Dialogs_BaseControl_DisableLocalization.md) | Отключить локализацию данного элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Dispose](M_TFlex_Dialogs_UiObject_Dispose.md) | (Унаследован от [UiObject](T_TFlex_Dialogs_UiObject.md)) |
|  | [Dispose(Boolean)](M_TFlex_Dialogs_BaseControl_Dispose.md) | (Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [EndUserEdit](M_TFlex_Dialogs_InputControlBase_EndUserEdit.md) | Завершить редактирование(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Dialogs_UiObject_Finalize.md) | (Унаследован от [UiObject](T_TFlex_Dialogs_UiObject.md)) |
|  | [Focus](M_TFlex_Dialogs_BaseControl_Focus.md) | Установить фокус ввода на элемент(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Increment](M_TFlex_Dialogs_NumericInputControl_Increment.md) | Увеличить текущее значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [Increment(Boolean)](M_TFlex_Dialogs_NumericInputControl_Increment_1.md) | Увеличить текущее значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveAllEventHandlers](M_TFlex_Dialogs_BaseControl_RemoveAllEventHandlers.md) | Отписать все подписанные обработчики событий(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [RevertChanges](M_TFlex_Dialogs_InputControlBase_RevertChanges.md) | Отменить изменения пользователя(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [Select](M_TFlex_Dialogs_InputControlBase_Select.md) | Выделить указанный текст(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [SelectAll](M_TFlex_Dialogs_InputControlBase_SelectAll.md) | Выделить весь текст(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [SetCustomLocalizationId(String)](M_TFlex_Dialogs_BaseControl_SetCustomLocalizationId.md) | Задать отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetCustomLocalizationId(String, Boolean)](M_TFlex_Dialogs_BaseControl_SetCustomLocalizationId_1.md) | Задать отдельный идентификатор для локализации(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SetDefaultValue(Double)](M_TFlex_Dialogs_NumericInputControl_SetDefaultValue.md) | Устанавливает значение по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetDefaultValue(Variable)](M_TFlex_Dialogs_NumericInputControl_SetDefaultValue_2.md) | Устанавливает значение по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetDefaultValue(Double, Unit)](M_TFlex_Dialogs_NumericInputControl_SetDefaultValue_1.md) | Устанавливает значение по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetDefaultValue(Variable, Unit)](M_TFlex_Dialogs_NumericInputControl_SetDefaultValue_3.md) | Устанавливает значение по умолчанию(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetMax(Double)](M_TFlex_Dialogs_NumericInputControl_SetMax.md) | Устанавливает максимальное допустимое значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetMax(Double, Boolean)](M_TFlex_Dialogs_NumericInputControl_SetMax_1.md) | Устанавливает максимальное допустимое значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetMin(Double)](M_TFlex_Dialogs_NumericInputControl_SetMin.md) | Устанавливает минимальное допустимое значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetMin(Double, Boolean)](M_TFlex_Dialogs_NumericInputControl_SetMin_1.md) | Устанавливает минимальное допустимое значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetRange(Range)](M_TFlex_Dialogs_NumericInputControl_SetRange_2.md) | Устанавливает диапазон допустимых значений(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetRange(Double, Double)](M_TFlex_Dialogs_NumericInputControl_SetRange.md) | Устанавливает диапазон допустимых значений(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetRange(Range, Boolean)](M_TFlex_Dialogs_NumericInputControl_SetRange_3.md) | Устанавливает диапазон допустимых значений(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetRange(Double, Double, Boolean)](M_TFlex_Dialogs_NumericInputControl_SetRange_1.md) | Устанавливает диапазон допустимых значений(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetValue(Double)](M_TFlex_Dialogs_NumericInputControl_SetValue.md) | Установить текущее значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetValue(Double, Variable)](M_TFlex_Dialogs_NumericInputControl_SetValue_1.md) | Установить текущее значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetValue(Double, Variable, Unit)](M_TFlex_Dialogs_NumericInputControl_SetValue_2.md) | Установить текущее значение(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetVariable(Variable)](M_TFlex_Dialogs_NumericInputControl_SetVariable.md) | Устанавливает текущую переменную(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SetVariable(Variable, Unit)](M_TFlex_Dialogs_NumericInputControl_SetVariable_1.md) | Устанавливает текущую переменную(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
|  | [SuppressEvents](M_TFlex_Dialogs_BaseControl_SuppressEvents.md) | Заглушить события(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [SuppressEvents(Boolean)](M_TFlex_Dialogs_BaseControl_SuppressEvents_1.md) | Заглушить события(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [UserIncrement](M_TFlex_Dialogs_NumericInputControl_UserIncrement.md) | Увеличить или уменьшить значение на UserIncrementStep заданное число раз(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activated](E_TFlex_Dialogs_BaseControl_Activated.md) | Событие активации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ActiveChanged](E_TFlex_Dialogs_BaseControl_ActiveChanged.md) | Событие активации либо деактивации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [AutocompleteFilling](E_TFlex_Dialogs_InputControlBase_AutocompleteFilling.md) | (Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [ChangesApplied](E_TFlex_Dialogs_InputControlBase_ChangesApplied.md) | Событие применения изменений(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [ChangesReverted](E_TFlex_Dialogs_InputControlBase_ChangesReverted.md) | События отмены изменений(Унаследован от [InputControlBase](T_TFlex_Dialogs_InputControlBase.md)) |
|  | [Deactivated](E_TFlex_Dialogs_BaseControl_Deactivated.md) | Событие деактивации элемента(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [FocusChanged](E_TFlex_Dialogs_BaseControl_FocusChanged.md) | Событие получения либо потери фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [GotFocus](E_TFlex_Dialogs_BaseControl_GotFocus.md) | Событие получения фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Locked](E_TFlex_Dialogs_BaseControl_Locked.md) | Событие установки флажка у чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LockedChanged](E_TFlex_Dialogs_BaseControl_LockedChanged.md) | Событие клика по чекбоксу метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [LostFocus](E_TFlex_Dialogs_BaseControl_LostFocus.md) | Событие потери фокуса ввода(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [Unlocked](E_TFlex_Dialogs_BaseControl_Unlocked.md) | Событие снятия флажка у чекбокса метки(Унаследован от [BaseControl](T_TFlex_Dialogs_BaseControl.md)) |
|  | [ValueChanged](E_TFlex_Dialogs_NumericInputControl_ValueChanged.md) | Событие изменения значения(Унаследован от [NumericInputControl](T_TFlex_Dialogs_NumericInputControl.md)) |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)