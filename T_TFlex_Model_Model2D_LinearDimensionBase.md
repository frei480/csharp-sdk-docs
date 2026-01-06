

Руководство по T-FLEX CAD Open API

# LinearDimensionBase - класс  
    
Базовый класс линейных размеров

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model2DObject2D](T_TFlex_Model_Model2D_Object2D.md) [TFlex.Model.Model2DDimension](T_TFlex_Model_Model2D_Dimension.md) TFlex.Model.Model2DLinearDimensionBase [TFlex.Model.Model2DLinearDimension](T_TFlex_Model_Model2D_LinearDimension.md) [TFlex.Model.Model3DLinearDimension3D](T_TFlex_Model_Model3D_LinearDimension3D.md) [TFlex.Model.Model3DProjectedLinearDimension](T_TFlex_Model_Model3D_ProjectedLinearDimension.md)

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class LinearDimensionBase : Dimension
```




Тип LinearDimensionBase предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [LinearDimensionBase(Document)](M_TFlex_Model_Model2D_LinearDimensionBase__ctor_2.md) | Инициализирует новый экземпляр класса LinearDimensionBase |
|  | [LinearDimensionBase(IntPtr)](M_TFlex_Model_Model2D_LinearDimensionBase__ctor.md) | Инициализирует новый экземпляр класса LinearDimensionBase |
|  | [LinearDimensionBase(IntPtr, Boolean)](M_TFlex_Model_Model2D_LinearDimensionBase__ctor_1.md) | Инициализирует новый экземпляр класса LinearDimensionBase |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Accuracy](P_TFlex_Model_Model2D_LinearDimensionBase_Accuracy.md) | Точность |
|  | [AltAccuracy](P_TFlex_Model_Model2D_LinearDimensionBase_AltAccuracy.md) | Точность для альтернативного размера |
|  | [AltLocation](P_TFlex_Model_Model2D_LinearDimensionBase_AltLocation.md) | Расположение альтернативного размера |
|  | [AltMinDigits](P_TFlex_Model_Model2D_LinearDimensionBase_AltMinDigits.md) | Минимальное количество знаков после запятой для альтернативного размера |
|  | [AltScaleFactor](P_TFlex_Model_Model2D_LinearDimensionBase_AltScaleFactor.md) | Величина дополнительного масштабирования альтернативного размера |
|  | [AltScaleFactorType](P_TFlex_Model_Model2D_LinearDimensionBase_AltScaleFactorType.md) | Тип дополнительного масштабирования альтернативного размера |
|  | [AltSeparator](P_TFlex_Model_Model2D_LinearDimensionBase_AltSeparator.md) | Тип разделителя для альтернативного размера |
|  | [AltTextAfter](P_TFlex_Model_Model2D_LinearDimensionBase_AltTextAfter.md) | Текст после числа альтернативного размера |
|  | [AltTextBefore](P_TFlex_Model_Model2D_LinearDimensionBase_AltTextBefore.md) | Текст перед числом альтернативного размера |
|  | [AltTextParameters](P_TFlex_Model_Model2D_LinearDimensionBase_AltTextParameters.md) | Параметры для отображения в тексте альтернативного размера |
|  | [AltTolerLetters](P_TFlex_Model_Model2D_LinearDimensionBase_AltTolerLetters.md) | Поле допуска с квалитетом для альтернативного размера |
|  | [AltTolerLowerDev](P_TFlex_Model_Model2D_LinearDimensionBase_AltTolerLowerDev.md) | Величина нижнего отклонения допуска для альтернативного размера |
|  | [AltTolerType](P_TFlex_Model_Model2D_LinearDimensionBase_AltTolerType.md) | Тип задания допуска для альтернативного размера |
|  | [AltTolerUpperDev](P_TFlex_Model_Model2D_LinearDimensionBase_AltTolerUpperDev.md) | Величина верхнего отклонения допуска для альтернативного размера |
|  | [AltUnits](P_TFlex_Model_Model2D_LinearDimensionBase_AltUnits.md) | Единицы измерения для альтернативного размера |
|  | [AltValueCorrection](P_TFlex_Model_Model2D_Dimension_AltValueCorrection.md) | Коррекция номинала альтернативного размера (применяется после применения масштаба)(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [BoundRect](P_TFlex_Model_Model2D_Object2D_BoundRect.md) | Получение координат прямоугольника, обрамляющего объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [BoxAroundText](P_TFlex_Model_Model2D_Dimension_BoxAroundText.md) | Рамка вокруг текста(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ClearUnderArrows](P_TFlex_Model_Model2D_Dimension_ClearUnderArrows.md) | Параметр очистки фона под стрелками и размерной линией(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ClearUnderEndArrow](P_TFlex_Model_Model2D_Dimension_ClearUnderEndArrow.md) | Параметр очистки фона под второй стрелкой(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ClearUnderLines](P_TFlex_Model_Model2D_Dimension_ClearUnderLines.md) | Параметр очистки фона под выносными линиями(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ClearUnderStartArrow](P_TFlex_Model_Model2D_Dimension_ClearUnderStartArrow.md) | Параметр очистки фона под первой стрелкой(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Color](P_TFlex_Model_Model2D_Dimension_Color.md) | Цвет объекта(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Dual](P_TFlex_Model_Model2D_LinearDimensionBase_Dual.md) | Режим отображения двойного размера |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [EndArrowSize](P_TFlex_Model_Model2D_LinearDimensionBase_EndArrowSize.md) | Размер конечной стрелки |
|  | [EndArrowType](P_TFlex_Model_Model2D_LinearDimensionBase_EndArrowType.md) | Тип конечной стрелки |
|  | [ExtOffset](P_TFlex_Model_Model2D_LinearDimensionBase_ExtOffset.md) | Величина смещения выносных линий |
|  | [FitLetters](P_TFlex_Model_Model2D_LinearDimensionBase_FitLetters.md) | Поле посадки с квалитетом |
|  | [FitLowerDev](P_TFlex_Model_Model2D_LinearDimensionBase_FitLowerDev.md) | Величина нижнего отклонения посадки |
|  | [FitUpperDev](P_TFlex_Model_Model2D_LinearDimensionBase_FitUpperDev.md) | Величина верхнего отклонения посадки |
|  | [FitView](P_TFlex_Model_Model2D_LinearDimensionBase_FitView.md) | Вид посадки |
|  | [FontStyle](P_TFlex_Model_Model2D_Dimension_FontStyle.md) | Получение стиля шрифта текста для получения или установки его параметров(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [GroupType](P_TFlex_Model_Model2D_Dimension_GroupType.md) | Тип объекта(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [HasSourceLines](P_TFlex_Model_Model2D_Dimension_HasSourceLines.md) | Проверить размер на возможность приведения параметра номинала размера к типу "По исходным линиям"(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model2D_Dimension_Layer.md) | Слой, на котором размещается объект(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Leader](P_TFlex_Model_Model2D_LinearDimensionBase_Leader.md) | Параметр отображения размера с выносной полкой |
|  | [LeaderDirection](P_TFlex_Model_Model2D_Dimension_LeaderDirection.md) | Направление полки с размерным числом(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Level](P_TFlex_Model_Model2D_Dimension_Level.md) | Уровень объекта(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [LinesType](P_TFlex_Model_Model2D_LinearDimensionBase_LinesType.md) | Режим отображения размерных и выносных линий |
|  | [ManualValue](P_TFlex_Model_Model2D_Dimension_ManualValue.md) | **Устарело.**(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ManualValueCorrection](P_TFlex_Model_Model2D_Dimension_ManualValueCorrection.md) | Использование заданного вручную значения коррекции размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [MinDigits](P_TFlex_Model_Model2D_LinearDimensionBase_MinDigits.md) | Минимальное число знаков после запятой |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [NominalOnlyText](P_TFlex_Model_Model2D_Dimension_NominalOnlyText.md) | Строка текста со значением только номинала размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Offset1](P_TFlex_Model_Model2D_Dimension_Offset1.md) | Отступ размера. Тип отступа зависит от типа размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Offset2](P_TFlex_Model_Model2D_Dimension_Offset2.md) | Отступ размера. Тип отступа зависит от типа размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Offset3](P_TFlex_Model_Model2D_Dimension_Offset3.md) | Отступ размера. Тип отступа зависит от типа размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [OutsideArrows](P_TFlex_Model_Model2D_LinearDimensionBase_OutsideArrows.md) | Состояние флага отображения стрелок с внешней стороны |
|  | [Page](P_TFlex_Model_Model2D_Dimension_Page.md) | Страница, на которой размещается элемент(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ParentDimension](P_TFlex_Model_Model2D_Dimension_ParentDimension.md) | Родительский размер(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PlaceFit](P_TFlex_Model_Model2D_LinearDimensionBase_PlaceFit.md) | Параметр отображения посадки |
|  | [PrefixSymbol](P_TFlex_Model_Model2D_LinearDimensionBase_PrefixSymbol.md) | Символ перед размерным числом |
|  | [Priority](P_TFlex_Model_Model2D_Dimension_Priority.md) | Приоритет объекта(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ScaleFactor](P_TFlex_Model_Model2D_LinearDimensionBase_ScaleFactor.md) | Величина дополнительного масштабирования размера |
|  | [ScaleFactorType](P_TFlex_Model_Model2D_LinearDimensionBase_ScaleFactorType.md) | Тип дополнительного масштабирования размера |
|  | [Standard](P_TFlex_Model_Model2D_LinearDimensionBase_Standard.md) | Тип стандарта размера |
|  | [StartArrowSize](P_TFlex_Model_Model2D_LinearDimensionBase_StartArrowSize.md) | Размер начальной стрелки |
|  | [StartArrowType](P_TFlex_Model_Model2D_LinearDimensionBase_StartArrowType.md) | Тип начальной стрелки |
|  | [State](P_TFlex_Model_Model2D_Dimension_State.md) | Тип положения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [StringsOffset](P_TFlex_Model_Model2D_LinearDimensionBase_StringsOffset.md) | Величина смещения строк от размерной линии |
|  | [SubType](P_TFlex_Model_Model2D_Dimension_SubType.md) | Подтип размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TextAfter](P_TFlex_Model_Model2D_Dimension_TextAfter.md) | Строка текста после текстом значения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TextBefore](P_TFlex_Model_Model2D_Dimension_TextBefore.md) | Строка текста перед текстом значения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TextParameters](P_TFlex_Model_Model2D_Dimension_TextParameters.md) | Способ отображения параметров размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TextUnder](P_TFlex_Model_Model2D_Dimension_TextUnder.md) | Строка текста под текстом значения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TolerAutomatic](P_TFlex_Model_Model2D_LinearDimensionBase_TolerAutomatic.md) | Параметр автоматического расчёта допуска |
|  | [TolerLetters](P_TFlex_Model_Model2D_LinearDimensionBase_TolerLetters.md) | Поле допуска с квалитетом |
|  | [TolerLowerDev](P_TFlex_Model_Model2D_LinearDimensionBase_TolerLowerDev.md) | Величина нижнего отклонения допуска |
|  | [TolerSize](P_TFlex_Model_Model2D_LinearDimensionBase_TolerSize.md) | Тип отображения допуска |
|  | [TolerUpperDev](P_TFlex_Model_Model2D_LinearDimensionBase_TolerUpperDev.md) | Величина верхнего отклонения допуска |
|  | [Units](P_TFlex_Model_Model2D_LinearDimensionBase_Units.md) | Единицы измерения |
|  | [Value](P_TFlex_Model_Model2D_Dimension_Value.md) | Численное значение размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ValueCorrection](P_TFlex_Model_Model2D_Dimension_ValueCorrection.md) | Коррекция номинала размера (применяется после применения масштаба)(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ValueText](P_TFlex_Model_Model2D_Dimension_ValueText.md) | Строка текста со значением размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ValueType](P_TFlex_Model_Model2D_Dimension_ValueType.md) | Способ формирования строки номинала размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_ModelObject_Clone.md) | Создаёт копию объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateObject](M_TFlex_Model_Model2D_Object2D_CreateObject.md) | (Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Draw](M_TFlex_Model_Model2D_Object2D_Draw.md) | Нарисовать объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetDistance](M_TFlex_Model_Model2D_Object2D_GetDistance.md) | Получение растояния до объекта(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetPoint](M_TFlex_Model_Model2D_Object2D_GetPoint.md) | Получение координат характерной точки объекта(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [GetPointCount](M_TFlex_Model_Model2D_Object2D_GetPointCount.md) | Получение количества характерных точек объекта, в которых может быть построен узел(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [GetPointID](M_TFlex_Model_Model2D_Object2D_GetPointID.md) | Получение идентификатора характерной точеки объекта с номером index(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [GetProperties](M_TFlex_Model_ModelObject_GetProperties.md) | Получить описание свойств элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealProp](M_TFlex_Model_ModelObject_GetRealProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealProperty](M_TFlex_Model_ModelObject_GetRealProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealPropertyWithUnit](M_TFlex_Model_ModelObject_GetRealPropertyWithUnit.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetReference(Int32)](M_TFlex_Model_ModelObject_GetReference.md) | Получить ссылку на родительский объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetReference_1.md) | Получить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetReferences](M_TFlex_Model_ModelObject_GetReferences.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRegenerationResult](M_TFlex_Model_ModelObject_GetRegenerationResult.md) | Результат пересчета объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRelation](M_TFlex_Model_ModelObject_GetRelation.md) | Измерить отношение двух объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRelationWithUnit](M_TFlex_Model_ModelObject_GetRelationWithUnit.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProp](M_TFlex_Model_ModelObject_GetTextProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProperty](M_TFlex_Model_ModelObject_GetTextProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InternalRegenerate](M_TFlex_Model_ModelObject_InternalRegenerate.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_Model2D_Dimension_OnEndChanges.md) | (Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ResetParameters](M_TFlex_Model_Model2D_Dimension_ResetParameters.md) | Установка параметров размера по-умолчанию(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [SetDefaults](M_TFlex_Model_Model2D_Dimension_SetDefaults.md) | Установка параметров размера в соответствии с параметрами по умолчанию(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetValue](M_TFlex_Model_Model2D_Dimension_SetValue.md) | Установка значения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Transform](M_TFlex_Model_Model2D_Object2D_Transform.md) | Применение преобразования.(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Translate](M_TFlex_Model_Model2D_Object2D_Translate.md) | Сдвиг объекта на данный вектор(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_AddMultilineText.md) | Аггрегировать новый многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineText.md) | Получить аггрегированный многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextBounds](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextBounds.md) | Получить габариты аггрегированного многострочного текста(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextsCount](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextsCount.md) | Количество аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [RemoveMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_RemoveMultilineText.md) | Удалить многострочный текст по индексу(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [UpdateMultilineTextPage](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_UpdateMultilineTextPage.md) | Обновить страницу аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)