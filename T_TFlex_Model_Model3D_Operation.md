

Руководство по T-FLEX CAD Open API

# Operation - класс  
    
Базовый класс для всех операций

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model3DObject3D](T_TFlex_Model_Model3D_Object3D.md) TFlex.Model.Model3DOperation Подробнее

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Operation : Object3D
```




Тип Operation предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Auxiliary](P_TFlex_Model_Model3D_Object3D_Auxiliary.md) | Внутрисистемный объект. Используется для Refer объектов фрагментов. Такие объекты скрыты от пользователя. Работа с такими объектами может быть реализована на уровне API.NET или ядром TFlex. Такие объекты не передаются на следующий уровень сборки. (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Body](P_TFlex_Model_Model3D_Operation_Body.md) | Тело, в которое входит операция |
|  | [CoatingMaterial](P_TFlex_Model_Model3D_Operation_CoatingMaterial.md) | Материал операции |
|  | [Color](P_TFlex_Model_Model3D_Object3D_Color.md) | Цвет(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ConstTransformations](P_TFlex_Model_Model3D_Object3D_ConstTransformations.md) | **Устарело.** Преобразование 3D объекта для чтения (устаревшая версия трансформации - допускается чтение трансформации в старых документах.)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Facet](P_TFlex_Model_Model3D_Operation_Facet.md) |  |
|  | [Fixed](P_TFlex_Model_Model3D_Operation_Fixed.md) | Свойство фиксации операции относительно сопряжений |
|  | [Geometry](P_TFlex_Model_Model3D_Operation_Geometry.md) | Геометрические данные операции |
|  | [GroupType](P_TFlex_Model_Model3D_Operation_GroupType.md) | Получить тип объекта(Переопределяет [ModelObjectGroupType](P_TFlex_Model_ModelObject_GroupType.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [InScene](P_TFlex_Model_Model3D_Object3D_InScene.md) | Объект в сцене(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTransparencyOn](P_TFlex_Model_Model3D_Operation_IsTransparencyOn.md) | Управление прозрачностью |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model3D_Object3D_Layer.md) | Слой, на котором размещается объект(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Level](P_TFlex_Model_Model3D_Object3D_Level.md) | Уровень(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Material](P_TFlex_Model_Model3D_Operation_Material.md) | Материал операции |
|  | [MaterialDistributionLaw](P_TFlex_Model_Model3D_Operation_MaterialDistributionLaw.md) |  |
|  | [MeshDensity](P_TFlex_Model_Model3D_Operation_MeshDensity.md) | Плотность сетки в диапазоне 0.0-1.0 |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Suppression](P_TFlex_Model_Model3D_Operation_Suppression.md) | Свойство подавленности операции |
|  | [TopLevel](P_TFlex_Model_Model3D_Operation_TopLevel.md) | Признак верхней операции |
|  | [TopOperation](P_TFlex_Model_Model3D_Operation_TopOperation.md) | Верхняя операция в теле |
|  | [Transformations](P_TFlex_Model_Model3D_Object3D_Transformations.md) | Контейнер групп преобразований 3D объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Transparency](P_TFlex_Model_Model3D_Operation_Transparency.md) | Прозрачность |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [VisibleInScene](P_TFlex_Model_Model3D_Object3D_VisibleInScene.md) | Свойство видимости объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [VolatileTransformations](P_TFlex_Model_Model3D_Object3D_VolatileTransformations.md) | **Устарело.** Преобразование 3D объекта для изменения(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Wireframe](P_TFlex_Model_Model3D_Operation_Wireframe.md) | Признак рёберной отрисовки операции |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CancelRollback](M_TFlex_Model_Model3D_Object3D_CancelRollback.md) | Завершить откат(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Clone](M_TFlex_Model_Model3D_Object3D_Clone.md) | Класс для передачи ссылки на геометрические свойства родительского объекта или на отдельные геометрические элементы тел модели (грани, циклы, рёбра, вершины)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateReference](M_TFlex_Model_Model3D_Object3D_CreateReference.md) | Создаёт ссылочный элемент в исходном документе(внутренняя ссылка)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CreateReference(Document)](M_TFlex_Model_Model3D_Object3D_CreateReference_1.md) | Создаёт ссылочный элемент в указанном документе(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DeleteMateTransformation](M_TFlex_Model_Model3D_Operation_DeleteMateTransformation.md) | Удалить текущее преобразование сопряжений |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ExportGeometry](M_TFlex_Model_Model3D_Operation_ExportGeometry.md) | Сохранение тел в файл в формате Parasolid |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindAssociatedTopols(Hole)](M_TFlex_Model_Model3D_Operation_FindAssociatedTopols.md) | Поиск топологических элементов, ассоциированных с отверстием |
|  | [FindAssociatedTopols(LCS)](M_TFlex_Model_Model3D_Operation_FindAssociatedTopols_1.md) | Поиск топологических элементов, ассоциированных с системой координат |
|  | [FindBodyOwner](M_TFlex_Model_Model3D_Operation_FindBodyOwner.md) | Получить базовую операцию, в которой хранятся свойства тела |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetGeomReference(Int32)](M_TFlex_Model_Model3D_Object3D_GetGeomReference.md) | Получить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetGeomReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_GetGeomReference_1.md) | Получить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetProperties](M_TFlex_Model_ModelObject_GetProperties.md) | Получить описание свойств элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealProp](M_TFlex_Model_ModelObject_GetRealProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealProperty](M_TFlex_Model_ModelObject_GetRealProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealPropertyWithUnit](M_TFlex_Model_ModelObject_GetRealPropertyWithUnit.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetReference(Int32)](M_TFlex_Model_Model3D_Object3D_GetReference.md) | Получить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_GetReference_1.md) | Получить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetReferences](M_TFlex_Model_ModelObject_GetReferences.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRegenerationResult](M_TFlex_Model_ModelObject_GetRegenerationResult.md) | Результат пересчета объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRelation](M_TFlex_Model_ModelObject_GetRelation.md) | Измерить отношение двух объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRelationWithUnit](M_TFlex_Model_ModelObject_GetRelationWithUnit.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProp](M_TFlex_Model_ModelObject_GetTextProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProperty](M_TFlex_Model_ModelObject_GetTextProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTransformationMatrix](M_TFlex_Model_Model3D_Object3D_GetTransformationMatrix.md) | (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InternalRegenerate](M_TFlex_Model_Model3D_Object3D_InternalRegenerate.md) | (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [LockMateTransformation](M_TFlex_Model_Model3D_Operation_LockMateTransformation.md) | Заблокировать текущее преобразование сопряжений от дальнейших изменений |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RadialRayTest](M_TFlex_Model_Model3D_Operation_RadialRayTest.md) |  |
|  | [RangePoint](M_TFlex_Model_Model3D_Operation_RangePoint.md) | Найти точку на операции ближайшую к данной точке |
|  | [RayTest(Operation, ValueType, ValueType)](M_TFlex_Model_Model3D_Operation_RayTest.md) |  |
|  | [RayTest(Operation, BasePoint3D, BaseDirection, ListDouble)](M_TFlex_Model_Model3D_Operation_RayTest_2.md) |  |
|  | [RayTest(Operation, ValueType, ValueType, Point3D, Double)](M_TFlex_Model_Model3D_Operation_RayTest_1.md) |  |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RollbackToParents](M_TFlex_Model_Model3D_Object3D_RollbackToParents.md) | Откат модели к состоянию, когда из сцены выгружены потомки объекта и он сам(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetGeomReference(Int32, Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_SetGeomReference.md) | Установить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetGeomReference(Int32, Object3DGeomReference, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_SetGeomReference_1.md) | Установить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_Model3D_Object3D_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetUniqueName](M_TFlex_Model_Model3D_Object3D_SetUniqueName.md) | Установить новое уникальное имя с заданным префиксом(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_AddMultilineText.md) | Аггрегировать новый многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineText.md) | Получить аггрегированный многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextBounds](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextBounds.md) | Получить габариты аггрегированного многострочного текста(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextsCount](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextsCount.md) | Количество аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [RemoveMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_RemoveMultilineText.md) | Удалить многострочный текст по индексу(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [UpdateMultilineTextPage](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_UpdateMultilineTextPage.md) | Обновить страницу аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
  
В текущей версии поддерживаются только листовые и твёрдотельные операции

#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model3DObject3D](T_TFlex_Model_Model3D_Object3D.md) TFlex.Model.Model3DOperation [TFlex.Model.Model3DArrayOperation](T_TFlex_Model_Model3D_ArrayOperation.md) [TFlex.Model.Model3DBasePipe](T_TFlex_Model_Model3D_BasePipe.md) [TFlex.Model.Model3DBend](T_TFlex_Model_Model3D_Bend.md) [TFlex.Model.Model3DBodyTaper](T_TFlex_Model_Model3D_BodyTaper.md) [TFlex.Model.Model3DBooleanOperation](T_TFlex_Model_Model3D_BooleanOperation.md) [TFlex.Model.Model3DCopyBaseOperation](T_TFlex_Model_Model3D_CopyBaseOperation.md) [TFlex.Model.Model3DCopyBaseOperation2](T_TFlex_Model_Model3D_CopyBaseOperation2.md) [TFlex.Model.Model3DCutOperation](T_TFlex_Model_Model3D_CutOperation.md) [TFlex.Model.Model3DEdgeBlending](T_TFlex_Model_Model3D_EdgeBlending.md) [TFlex.Model.Model3DExtendSurface](T_TFlex_Model_Model3D_ExtendSurface.md) [TFlex.Model.Model3DExternalOperation](T_TFlex_Model_Model3D_ExternalOperation.md) [TFlex.Model.Model3DFaceBlending](T_TFlex_Model_Model3D_FaceBlending.md) [TFlex.Model.Model3DFaceChange](T_TFlex_Model_Model3D_FaceChange.md) [TFlex.Model.Model3DFaceDelete](T_TFlex_Model_Model3D_FaceDelete.md) [TFlex.Model.Model3DFaceReplace](T_TFlex_Model_Model3D_FaceReplace.md) [TFlex.Model.Model3DFaceSeparate](T_TFlex_Model_Model3D_FaceSeparate.md) [TFlex.Model.Model3DFaceTransform](T_TFlex_Model_Model3D_FaceTransform.md) [TFlex.Model.Model3DFillHole](T_TFlex_Model_Model3D_FillHole.md) [TFlex.Model.Model3DFillHoleOperation](T_TFlex_Model_Model3D_FillHoleOperation.md) [TFlex.Model.Model3DFragment3D](T_TFlex_Model_Model3D_Fragment3D.md) [TFlex.Model.Model3DHole](T_TFlex_Model_Model3D_Hole.md) [TFlex.Model.Model3DImportedOperation](T_TFlex_Model_Model3D_ImportedOperation.md) [TFlex.Model.Model3DImprint](T_TFlex_Model_Model3D_Imprint.md) [TFlex.Model.Model3DLoft](T_TFlex_Model_Model3D_Loft.md) [TFlex.Model.Model3DLoftOperation](T_TFlex_Model_Model3D_LoftOperation.md) [TFlex.Model.Model3DMaterialOperation](T_TFlex_Model_Model3D_MaterialOperation.md) [TFlex.Model.Model3DOffset](T_TFlex_Model_Model3D_Offset.md) [TFlex.Model.Model3DOffsetSurf](T_TFlex_Model_Model3D_OffsetSurf.md) [TFlex.Model.Model3DParametricArrayOperation](T_TFlex_Model_Model3D_ParametricArrayOperation.md) [TFlex.Model.Model3DPrimitive](T_TFlex_Model_Model3D_Primitive.md) [TFlex.Model.Model3DRebend](T_TFlex_Model_Model3D_Rebend.md) [TFlex.Model.Model3DReferenceOperation](T_TFlex_Model_Model3D_ReferenceOperation.md) [TFlex.Model.Model3DSeparation](T_TFlex_Model_Model3D_Separation.md) [TFlex.Model.Model3DSew](T_TFlex_Model_Model3D_Sew.md) [TFlex.Model.Model3DSheetMetalFeature](T_TFlex_Model_Model3D_SheetMetalFeature.md) [TFlex.Model.Model3DSheetMetalPart](T_TFlex_Model_Model3D_SheetMetalPart.md) [TFlex.Model.Model3DShell](T_TFlex_Model_Model3D_Shell.md) [TFlex.Model.Model3DSimplification](T_TFlex_Model_Model3D_Simplification.md) [TFlex.Model.Model3DSpiral](T_TFlex_Model_Model3D_Spiral.md) [TFlex.Model.Model3DSpring](T_TFlex_Model_Model3D_Spring.md) [TFlex.Model.Model3DSweep](T_TFlex_Model_Model3D_Sweep.md) [TFlex.Model.Model3DTaper](T_TFlex_Model_Model3D_Taper.md) [TFlex.Model.Model3DThread](T_TFlex_Model_Model3D_Thread.md) [TFlex.Model.Model3DThreeFaceBlending](T_TFlex_Model_Model3D_ThreeFaceBlending.md) [TFlex.Model.Model3DUnbend](T_TFlex_Model_Model3D_Unbend.md)