

Руководство по T-FLEX CAD Open API

# FaceBlending - класс  
    
Сглаживание граней

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model3DObject3D](T_TFlex_Model_Model3D_Object3D.md) [TFlex.Model.Model3DOperation](T_TFlex_Model_Model3D_Operation.md) TFlex.Model.Model3DFaceBlending

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class FaceBlending : Operation
```




Тип FaceBlending предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [FaceBlending](M_TFlex_Model_Model3D_FaceBlending__ctor.md) | Конструктор для создания операции "Сглаживание граней" |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Attribute](P_TFlex_Model_Model3D_FaceBlending_Attribute.md) | Атрибут сглаживания |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Auxiliary](P_TFlex_Model_Model3D_Object3D_Auxiliary.md) | Внутрисистемный объект. Используется для Refer объектов фрагментов. Такие объекты скрыты от пользователя. Работа с такими объектами может быть реализована на уровне API.NET или ядром TFlex. Такие объекты не передаются на следующий уровень сборки. (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [BlendTrim](P_TFlex_Model_Model3D_FaceBlending_BlendTrim.md) | Тип торца |
|  | [BlendWalls](P_TFlex_Model_Model3D_FaceBlending_BlendWalls.md) | Тип результата |
|  | [Body](P_TFlex_Model_Model3D_Operation_Body.md) | Тело, в которое входит операция(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [CoatingMaterial](P_TFlex_Model_Model3D_Operation_CoatingMaterial.md) | Материал операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Color](P_TFlex_Model_Model3D_Object3D_Color.md) | Цвет(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ConstraintLimit1](P_TFlex_Model_Model3D_FaceBlending_ConstraintLimit1.md) | Первая ограничивающая плоскость |
|  | [ConstraintLimit2](P_TFlex_Model_Model3D_FaceBlending_ConstraintLimit2.md) | Вторая ограничивающая плоскость |
|  | [ConstTransformations](P_TFlex_Model_Model3D_Object3D_ConstTransformations.md) | **Устарело.** Преобразование 3D объекта для чтения (устаревшая версия трансформации - допускается чтение трансформации в старых документах.)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CrossSectionPlaneMethod](P_TFlex_Model_Model3D_FaceBlending_CrossSectionPlaneMethod.md) | Тип плоскости пересечения секций |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Facet](P_TFlex_Model_Model3D_Operation_Facet.md) | (Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [FFBlendOperGet](P_TFlex_Model_Model3D_FaceBlending_FFBlendOperGet.md) |  |
|  | [FFBlendOperSet](P_TFlex_Model_Model3D_FaceBlending_FFBlendOperSet.md) |  |
|  | [Fixed](P_TFlex_Model_Model3D_Operation_Fixed.md) | Свойство фиксации операции относительно сопряжений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Geometry](P_TFlex_Model_Model3D_Operation_Geometry.md) | Геометрические данные операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [GroupType](P_TFlex_Model_Model3D_FaceBlending_GroupType.md) | Получить тип объекта(Переопределяет [OperationGroupType](P_TFlex_Model_Model3D_Operation_GroupType.md)) |
|  | [HelpPoint](P_TFlex_Model_Model3D_FaceBlending_HelpPoint.md) | Вспомогательная точка |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [InScene](P_TFlex_Model_Model3D_Object3D_InScene.md) | Объект в сцене(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTransparencyOn](P_TFlex_Model_Model3D_Operation_IsTransparencyOn.md) | Управление прозрачностью(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model3D_Object3D_Layer.md) | Слой, на котором размещается объект(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [LeftSense](P_TFlex_Model_Model3D_FaceBlending_LeftSense.md) | Реверс левой стенки |
|  | [Level](P_TFlex_Model_Model3D_Object3D_Level.md) | Уровень(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Material](P_TFlex_Model_Model3D_Operation_Material.md) | Материал операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MaterialDistributionLaw](P_TFlex_Model_Model3D_Operation_MaterialDistributionLaw.md) | (Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MeshDensity](P_TFlex_Model_Model3D_Operation_MeshDensity.md) | Плотность сетки в диапазоне 0.0-1.0(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [NotchFlag](P_TFlex_Model_Model3D_FaceBlending_NotchFlag.md) | Параметр "Вырез" |
|  | [NumberOfConstraintEdges](P_TFlex_Model_Model3D_FaceBlending_NumberOfConstraintEdges.md) | Получить число ограничивающих рёбер |
|  | [NumberOfLeftFaces](P_TFlex_Model_Model3D_FaceBlending_NumberOfLeftFaces.md) | Получить число граней образующих левую стенку |
|  | [NumberOfRightFaces](P_TFlex_Model_Model3D_FaceBlending_NumberOfRightFaces.md) | Получить число граней образующих правую стенку |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PropagateFlag](P_TFlex_Model_Model3D_FaceBlending_PropagateFlag.md) | Параметр "Продолжить по касательной" |
|  | [RightSense](P_TFlex_Model_Model3D_FaceBlending_RightSense.md) | Реверс правой стенки |
|  | [Spine](P_TFlex_Model_Model3D_FaceBlending_Spine.md) | Путь |
|  | [Suppression](P_TFlex_Model_Model3D_Operation_Suppression.md) | Свойство подавленности операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [TopLevel](P_TFlex_Model_Model3D_Operation_TopLevel.md) | Признак верхней операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [TopOperation](P_TFlex_Model_Model3D_Operation_TopOperation.md) | Верхняя операция в теле(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Transformations](P_TFlex_Model_Model3D_Object3D_Transformations.md) | Контейнер групп преобразований 3D объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Transparency](P_TFlex_Model_Model3D_Operation_Transparency.md) | Прозрачность(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [UseHelpPoint](P_TFlex_Model_Model3D_FaceBlending_UseHelpPoint.md) | Параметр использования вспомогательной точки |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [VisibleInScene](P_TFlex_Model_Model3D_Object3D_VisibleInScene.md) | Свойство видимости объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [VolatileTransformations](P_TFlex_Model_Model3D_Object3D_VolatileTransformations.md) | **Устарело.** Преобразование 3D объекта для изменения(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Wireframe](P_TFlex_Model_Model3D_Operation_Wireframe.md) | Признак рёберной отрисовки операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddConstraintEdge](M_TFlex_Model_Model3D_FaceBlending_AddConstraintEdge.md) | Добавить ограничивающее ребро |
|  | [AddLeftFace](M_TFlex_Model_Model3D_FaceBlending_AddLeftFace.md) | Добавить грань в левую стенку |
|  | [AddRightFace](M_TFlex_Model_Model3D_FaceBlending_AddRightFace.md) | Добавить грань в правую стенку |
|  | [CancelRollback](M_TFlex_Model_Model3D_Object3D_CancelRollback.md) | Завершить откат(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Clone](M_TFlex_Model_Model3D_Object3D_Clone.md) | Класс для передачи ссылки на геометрические свойства родительского объекта или на отдельные геометрические элементы тел модели (грани, циклы, рёбра, вершины)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateReference](M_TFlex_Model_Model3D_Object3D_CreateReference.md) | Создаёт ссылочный элемент в исходном документе(внутренняя ссылка)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CreateReference(Document)](M_TFlex_Model_Model3D_Object3D_CreateReference_1.md) | Создаёт ссылочный элемент в указанном документе(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DeleteMateTransformation](M_TFlex_Model_Model3D_Operation_DeleteMateTransformation.md) | Удалить текущее преобразование сопряжений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ExportGeometry](M_TFlex_Model_Model3D_Operation_ExportGeometry.md) | Сохранение тел в файл в формате Parasolid(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindAssociatedTopols(Hole)](M_TFlex_Model_Model3D_Operation_FindAssociatedTopols.md) | Поиск топологических элементов, ассоциированных с отверстием(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [FindAssociatedTopols(LCS)](M_TFlex_Model_Model3D_Operation_FindAssociatedTopols_1.md) | Поиск топологических элементов, ассоциированных с системой координат(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [FindBodyOwner](M_TFlex_Model_Model3D_Operation_FindBodyOwner.md) | Получить базовую операцию, в которой хранятся свойства тела(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetGeomReference(Int32)](M_TFlex_Model_Model3D_Object3D_GetGeomReference.md) | Получить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetGeomReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_GetGeomReference_1.md) | Получить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetLeftFace](M_TFlex_Model_Model3D_FaceBlending_GetLeftFace.md) | Полуить левую грань |
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
|  | [GetRightFace](M_TFlex_Model_Model3D_FaceBlending_GetRightFace.md) | Полуить правую грань |
|  | [GetTextProp](M_TFlex_Model_ModelObject_GetTextProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProperty](M_TFlex_Model_ModelObject_GetTextProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTransformationMatrix](M_TFlex_Model_Model3D_Object3D_GetTransformationMatrix.md) | (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InternalRegenerate](M_TFlex_Model_Model3D_Object3D_InternalRegenerate.md) | (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [LockMateTransformation](M_TFlex_Model_Model3D_Operation_LockMateTransformation.md) | Заблокировать текущее преобразование сопряжений от дальнейших изменений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RemoveAllConstraintEdges](M_TFlex_Model_Model3D_FaceBlending_RemoveAllConstraintEdges.md) | Удалить все ограничивающие рёбра |
|  | [RemoveAllLeftFaces](M_TFlex_Model_Model3D_FaceBlending_RemoveAllLeftFaces.md) | Удалить грани образующие левую стенку |
|  | [RemoveAllRightFaces](M_TFlex_Model_Model3D_FaceBlending_RemoveAllRightFaces.md) | Удалить грани образующие правую стенку |
|  | [RemoveConstraintEdge](M_TFlex_Model_Model3D_FaceBlending_RemoveConstraintEdge.md) | Удалить ограничивающее ребро |
|  | [RemoveLeftFace](M_TFlex_Model_Model3D_FaceBlending_RemoveLeftFace.md) | Удалить левую грань |
|  | [RemoveRightFace](M_TFlex_Model_Model3D_FaceBlending_RemoveRightFace.md) | Удалить правую грань |
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
      
    
    public static void FaceBlending()
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("операция сглаживания граней");//Открытие блока изменений документа
    
       //путь
       PathConstruction pathConstruction = new PathConstruction(document);
       TFlex.Model.Model2D.Contour cn = pathConstruction.Contour;//контур
    
       //создание узлов
       FreeNode fn1 = new FreeNode(document, -200, 50);            
       FreeNode fn2 = new FreeNode(document, -160, 100);
       FreeNode fn3 = new FreeNode(document, -120, 50);            
       FreeNode fn4 = new FreeNode(document, -80, 100);  
    
       //соединяем узлы линиями
       ConstructionOutline l1 = new ConstructionOutline(document, fn1, fn2);
       ConstructionOutline l2 = new ConstructionOutline(document, fn2, fn3);
       ConstructionOutline l3 = new ConstructionOutline(document, fn3, fn4);
    
       double r = 68;    
    
       //дуга окружности, проходящая через два узла с заданным радиусом
       TwoPointArcOutline twoPointArcOutline = new TwoPointArcOutline(document, fn4, fn1, r);    
    
       //отнесение этих линий к контуру 
       OutlineContourSegment s1 = new OutlineContourSegment(cn);
       OutlineContourSegment s2 = new OutlineContourSegment(cn);
       OutlineContourSegment s3 = new OutlineContourSegment(cn);
       OutlineContourSegment s4 = new OutlineContourSegment(cn);             
       s1.Outline = l1; s2.Outline = l2; s3.Outline = l3;s4.Outline = twoPointArcOutline;  
    
       //создание штриховки
       Area ar = new Area (document); 
       TFlex.Model.Model2D.Contour cn1 = ar.AppendContour(); 
       //путь - контур штирховки
       ConstructionContourSegment seg1 = new ConstructionContourSegment(cn1); 
       seg1.Construction = pathConstruction; 
    
       //построение профиля
       StandardWorkplane swp = new StandardWorkplane(document, StandardWorkplane.StandardType.Left); 
       AreaProfile areaProfile = new AreaProfile(document); 
       areaProfile.Area = ar; //профиль по штриховке
       areaProfile.WorkSurface = swp;//Рабочая поверхность, задающая ориентацию профиля
    
       //выталкивание
       ThickenExtrusion ex = new ThickenExtrusion(document); 
       ex.Thickness1 = 10; 
       ex.LengthType = ThickenExtrusion.LengthValue.AutoValue; //Данный параметр должен быть выставлен! 
       ex.ForwardLength = 50; 
       ex.Profile.Add(areaProfile.Geometry.SheetContour);     
    
       document.ApplyChanges();//Применить изменения без закрытия блока изменения документа           
       FaceBlending faceBlending = new FaceBlending(document);//операция сглаживания
    
       int r = 30;//радиус сглаживания
       //класс свойств, используемый для создания сглаживания с постоянным радиусом
       TFlex.Model.Model3D.FaceBlending.ContinuousRadiusAttribute s = new TFlex.Model.Model3D.FaceBlending.ContinuousRadiusAttribute(r);
       faceBlending.Attribute = s;//установка радиуса для операции    
    
       //грани тела выталкивания
       faceBlending.AddLeftFace((ModelFace)ex.Geometry.Solid[0].Faces[0]);
       faceBlending.AddRightFace((ModelFace)ex.Geometry.Solid[0].Faces[1]);    
    
       //реверс этих граней
       faceBlending.LeftSense = true;
       faceBlending.RightSense = true;
       faceBlending.BlendWalls = FaceBlending.WallsType.Solid;//тип результата - отдельное тело
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)