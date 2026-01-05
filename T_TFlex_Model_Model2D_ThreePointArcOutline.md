

Руководство по T-FLEX CAD Open API

# ThreePointArcOutline - класс  
  
---  
  
Линия изображения - дуга окружности, проходящая через три узла

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model2DObject2D](T_TFlex_Model_Model2D_Object2D.md) [TFlex.Model.Model2DOutline](T_TFlex_Model_Model2D_Outline.md) TFlex.Model.Model2DThreePointArcOutline

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class ThreePointArcOutline : Outline
```
```vb
Public Class ThreePointArcOutline
	Inherits Outline
```
```cpp
public ref class ThreePointArcOutline : public Outline
```


Тип ThreePointArcOutline предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ThreePointArcOutline](M_TFlex_Model_Model2D_ThreePointArcOutline__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [BoundRect](P_TFlex_Model_Model2D_Object2D_BoundRect.md) | Получение координат прямоугольника, обрамляющего объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Color](P_TFlex_Model_Model2D_Outline_Color.md) | Цвет линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [EndArrowSize](P_TFlex_Model_Model2D_Outline_EndArrowSize.md) | Размер конечной стрелки линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [EndArrowType](P_TFlex_Model_Model2D_Outline_EndArrowType.md) | Тип конечной стрелки линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [EndNode](P_TFlex_Model_Model2D_ThreePointArcOutline_EndNode.md) | Конечный узел дуги |
|  | [Geometry](P_TFlex_Model_Model2D_Outline_Geometry.md) | Получение геометрии линии изображения с учётом масштаба(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [GeometryAsPolyline](P_TFlex_Model_Model2D_Outline_GeometryAsPolyline.md) | Получение геометрии в виде полилинии независимо от типа(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [GeometryType](P_TFlex_Model_Model2D_Outline_GeometryType.md) | Тип геометрии линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [GroupType](P_TFlex_Model_Model2D_Outline_GroupType.md) | Тип объекта "Линия изображения"(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsService](P_TFlex_Model_Model2D_Outline_IsService.md) | Вспомогательная линия(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model2D_Outline_Layer.md) | Слой линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [Level](P_TFlex_Model_Model2D_Outline_Level.md) | Уровень линии(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [LineWidth](P_TFlex_Model_Model2D_Outline_LineWidth.md) | Толщина линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [MiddleNode](P_TFlex_Model_Model2D_ThreePointArcOutline_MiddleNode.md) | Узел, через который проходит дуга |
|  | [ModelGeometry](P_TFlex_Model_Model2D_Outline_ModelGeometry.md) | Получение геометрии линии изображения без учёта масштаба(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Page](P_TFlex_Model_Model2D_Outline_Page.md) | Страница линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PatternName](P_TFlex_Model_Model2D_Outline_PatternName.md) | Имя образца штриховой линии(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [PatternScale](P_TFlex_Model_Model2D_Outline_PatternScale.md) | Масштаб штрихов штриховой линии(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [Priority](P_TFlex_Model_Model2D_Outline_Priority.md) | Приоритет линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [StartArrowSize](P_TFlex_Model_Model2D_Outline_StartArrowSize.md) | Размер начальной стрелки линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [StartArrowType](P_TFlex_Model_Model2D_Outline_StartArrowType.md) | Тип начальной стрелки линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [StartNode](P_TFlex_Model_Model2D_ThreePointArcOutline_StartNode.md) | Начальный узел дуги |
|  | [Style](P_TFlex_Model_Model2D_Outline_Style.md) | Стиль линии изображения(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [SubType](P_TFlex_Model_Model2D_ThreePointArcOutline_SubType.md) | Подтип линии изображения(Переопределяет [OutlineSubType](P_TFlex_Model_Model2D_Outline_SubType.md)) |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [WaveHeight](P_TFlex_Model_Model2D_Outline_WaveHeight.md) | Высота волны волнистой линии(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [WaveLength](P_TFlex_Model_Model2D_Outline_WaveLength.md) | Длина волны волнистой линии(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [WaveNumber](P_TFlex_Model_Model2D_Outline_WaveNumber.md) | Количество волн волнистой линии(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [WaveSetting](P_TFlex_Model_Model2D_Outline_WaveSetting.md) | Способ задания волнистой линии(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_ModelObject_Clone.md) | Создаёт копию объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateDefaultStyle](M_TFlex_Model_Model2D_Outline_CreateDefaultStyle.md) | (Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [CreateDefaultStyleForAxes](M_TFlex_Model_Model2D_Outline_CreateDefaultStyleForAxes.md) | (Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [CreateObject](M_TFlex_Model_Model2D_Object2D_CreateObject.md) | (Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Draw](M_TFlex_Model_Model2D_Object2D_Draw.md) | Нарисовать объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [EvaluatePoint](M_TFlex_Model_Model2D_Outline_EvaluatePoint.md) | Получить точку на кривой по параметру iU (Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetDashStyle](M_TFlex_Model_Model2D_Outline_GetDashStyle.md) | Получение штрихов(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
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
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetDashStyle](M_TFlex_Model_Model2D_Outline_SetDashStyle.md) | (Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [SetDefaults](M_TFlex_Model_Model2D_Outline_SetDefaults.md) | Установка параметров линий изображения в соответствии с параметрами по умолчанию(Унаследован от [Outline](T_TFlex_Model_Model2D_Outline.md)) |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
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
      
    
    public static void ThreePointArcOutline()
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");//Открытие блока изменений документа
    
       FreeNode fn1 = new FreeNode(document, 450, 320);            
       FreeNode fn2 = new FreeNode(document, 470, 340);            
       FreeNode fn3 = new FreeNode(document, 490, 320);            
       ThreePointArcOutline threePointArcOutline = new ThreePointArcOutline(document, fn1, fn2, fn3);//дуга окружности, проходящая через три узла
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)