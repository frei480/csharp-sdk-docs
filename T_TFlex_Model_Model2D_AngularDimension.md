

Руководство по T-FLEX CAD Open API

# AngularDimension - класс  
    
Угловой размер на 2D

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model2DObject2D](T_TFlex_Model_Model2D_Object2D.md) [TFlex.Model.Model2DDimension](T_TFlex_Model_Model2D_Dimension.md) [TFlex.Model.Model2DAngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md) TFlex.Model.Model2DAngularDimension

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class AngularDimension : AngularDimensionBase
```
```vb
Public Class AngularDimension
	Inherits AngularDimensionBase
```
```cpp
public ref class AngularDimension : public AngularDimensionBase
```


Тип AngularDimension предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [AngularDimension](M_TFlex_Model_Model2D_AngularDimension__ctor.md) | Конструктор по умолчанию |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Accuracy](P_TFlex_Model_Model2D_AngularDimensionBase_Accuracy.md) | Точность(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [AltValueCorrection](P_TFlex_Model_Model2D_Dimension_AltValueCorrection.md) | Коррекция номинала альтернативного размера (применяется после применения масштаба)(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [AngularDimType](P_TFlex_Model_Model2D_AngularDimension_AngularDimType.md) | Подтип углового размера |
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
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [EndArrowSize](P_TFlex_Model_Model2D_AngularDimensionBase_EndArrowSize.md) | Размер конечной стрелки(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [EndArrowType](P_TFlex_Model_Model2D_AngularDimensionBase_EndArrowType.md) | Тип конечной стрелки(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [ExtOffset](P_TFlex_Model_Model2D_AngularDimensionBase_ExtOffset.md) | Величина смещения выносных линий(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [FontStyle](P_TFlex_Model_Model2D_Dimension_FontStyle.md) | Получение стиля шрифта текста для получения или установки его параметров(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [GroupType](P_TFlex_Model_Model2D_Dimension_GroupType.md) | Тип объекта(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [HasSourceLines](P_TFlex_Model_Model2D_Dimension_HasSourceLines.md) | Проверить размер на возможность приведения параметра номинала размера к типу "По исходным линиям"(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model2D_Dimension_Layer.md) | Слой, на котором размещается объект(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [LeaderDirection](P_TFlex_Model_Model2D_Dimension_LeaderDirection.md) | Направление полки с размерным числом(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Level](P_TFlex_Model_Model2D_Dimension_Level.md) | Уровень объекта(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [LinesType](P_TFlex_Model_Model2D_AngularDimensionBase_LinesType.md) | Режим отображения размерных и выносных линий(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [ManualValue](P_TFlex_Model_Model2D_Dimension_ManualValue.md) | **Устарело.**(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ManualValueCorrection](P_TFlex_Model_Model2D_Dimension_ManualValueCorrection.md) | Использование заданного вручную значения коррекции размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [MinDigits](P_TFlex_Model_Model2D_AngularDimensionBase_MinDigits.md) | Минимальное число знаков после запятой(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [NominalOnlyText](P_TFlex_Model_Model2D_Dimension_NominalOnlyText.md) | Строка текста со значением только номинала размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Offset1](P_TFlex_Model_Model2D_Dimension_Offset1.md) | Отступ размера. Тип отступа зависит от типа размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Offset2](P_TFlex_Model_Model2D_Dimension_Offset2.md) | Отступ размера. Тип отступа зависит от типа размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Offset3](P_TFlex_Model_Model2D_Dimension_Offset3.md) | Отступ размера. Тип отступа зависит от типа размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [OutsideArrows](P_TFlex_Model_Model2D_AngularDimensionBase_OutsideArrows.md) | Состояние флага отображения стрелок с внешней стороны(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [Page](P_TFlex_Model_Model2D_Dimension_Page.md) | Страница, на которой размещается элемент(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ParentDimension](P_TFlex_Model_Model2D_Dimension_ParentDimension.md) | Родительский размер(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Priority](P_TFlex_Model_Model2D_Dimension_Priority.md) | Приоритет объекта(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [Standard](P_TFlex_Model_Model2D_AngularDimensionBase_Standard.md) | Тип стандарта размера(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [StartArrowSize](P_TFlex_Model_Model2D_AngularDimensionBase_StartArrowSize.md) | Размер начальной стрелки(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [StartArrowType](P_TFlex_Model_Model2D_AngularDimensionBase_StartArrowType.md) | Тип начальной стрелки(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [State](P_TFlex_Model_Model2D_Dimension_State.md) | Тип положения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [StringsOffset](P_TFlex_Model_Model2D_AngularDimensionBase_StringsOffset.md) | Величина смещения строк от размерной линии(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [SubType](P_TFlex_Model_Model2D_AngularDimension_SubType.md) | Подтип размера(Переопределяет [DimensionSubType](P_TFlex_Model_Model2D_Dimension_SubType.md)) |
|  | [TextAfter](P_TFlex_Model_Model2D_Dimension_TextAfter.md) | Строка текста после текстом значения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TextBefore](P_TFlex_Model_Model2D_Dimension_TextBefore.md) | Строка текста перед текстом значения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TextOnLine](P_TFlex_Model_Model2D_AngularDimension_TextOnLine.md) | Текст вдоль линии, а не по дуге |
|  | [TextParameters](P_TFlex_Model_Model2D_Dimension_TextParameters.md) | Способ отображения параметров размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TextUnder](P_TFlex_Model_Model2D_Dimension_TextUnder.md) | Строка текста под текстом значения размера(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [TolerAutomatic](P_TFlex_Model_Model2D_AngularDimensionBase_TolerAutomatic.md) | Указывает на то, что допуск будет рассчитываться автоматически(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [TolerLowerDev](P_TFlex_Model_Model2D_AngularDimensionBase_TolerLowerDev.md) | Величина нижнего отклонения допуска(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [TolerUpperDev](P_TFlex_Model_Model2D_AngularDimensionBase_TolerUpperDev.md) | Величина верхнего отклонения допуска(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
|  | [Units](P_TFlex_Model_Model2D_AngularDimensionBase_Units.md) | Тип единиц измерения(Унаследован от [AngularDimensionBase](T_TFlex_Model_Model2D_AngularDimensionBase.md)) |
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
|  | [SetConstructionAndOutline](M_TFlex_Model_Model2D_AngularDimension_SetConstructionAndOutline.md) | Установка параметров размера между линией построения и линией изображения |
|  | [SetDefaults](M_TFlex_Model_Model2D_Dimension_SetDefaults.md) | Установка параметров размера в соответствии с параметрами по умолчанию(Унаследован от [Dimension](T_TFlex_Model_Model2D_Dimension.md)) |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetLeaderNote](M_TFlex_Model_Model2D_AngularDimension_SetLeaderNote.md) | Установка привязок размера к узлам, либо по относительным смещениям |
|  | [SetOffsets](M_TFlex_Model_Model2D_AngularDimension_SetOffsets.md) | Установка привязок размера к узлам, либо по относительным смещениям |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetTwoConstructions](M_TFlex_Model_Model2D_AngularDimension_SetTwoConstructions.md) | Установка параметров размера между двумя линиями построения |
|  | [SetTwoOutlines](M_TFlex_Model_Model2D_AngularDimension_SetTwoOutlines.md) | Установка параметров размера между двумя линиями изображения |
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
      
    
    public static void AngularDimension()
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("Размер");//Открытие блока изменений документа
    
       FreeNode fn1 = new FreeNode(document, 300, 400);//создание узла            
       FreeNode fn2 = new FreeNode(document, 400, 500);
    
       FreeNode fn3 = new FreeNode(document, 400, 400);//создание узла            
       FreeNode fn4 = new FreeNode(document, 300, 480);
    
       LineConstruction l1 = new LineConstruction(document);//прямая1
       l1.SetThroughNodes(fn1, fn2);  
    
       LineConstruction l2 = new LineConstruction(document);//прямая2
       l2.SetThroughNodes(fn3, fn4);  
    
       AngularDimension a = new AngularDimension(document);//угловой размер
       //размер между двумя линиями изображения
       //(прямая1, начало выносной линии на прямой, прямая2, начало выносной линии на прямой, 
       // положения угловых размеров-между положительными направлениями линий(AnglePosition.BetweenHeadAndHead))
       a.SetTwoConstructions(l1, fn1, l2, fn3, AnglePosition.BetweenHeadAndHead);
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)