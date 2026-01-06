

Руководство по T-FLEX CAD Open API

# Loft - класс  
    
**Примечание: Данный API устарел.**

Операция "по сечениям"

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model3DObject3D](T_TFlex_Model_Model3D_Object3D.md) [TFlex.Model.Model3DOperation](T_TFlex_Model_Model3D_Operation.md) TFlex.Model.Model3DLoft

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This class is obsolete and will be removed. Please use 'LoftOperation' class.")]
public class Loft : Operation
```
```vb
<ObsoleteAttribute("This class is obsolete and will be removed. Please use 'LoftOperation' class.")>
Public Class Loft
	Inherits Operation
```
```cpp
[ObsoleteAttribute(L"This class is obsolete and will be removed. Please use 'LoftOperation' class.")]
public ref class Loft : public Operation
```


Тип Loft предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Loft](M_TFlex_Model_Model3D_Loft__ctor.md) | Конструктор для создания Лофтинга |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Auxiliary](P_TFlex_Model_Model3D_Object3D_Auxiliary.md) | Внутрисистемный объект. Используется для Refer объектов фрагментов. Такие объекты скрыты от пользователя. Работа с такими объектами может быть реализована на уровне API.NET или ядром TFlex. Такие объекты не передаются на следующий уровень сборки. (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Body](P_TFlex_Model_Model3D_Operation_Body.md) | Тело, в которое входит операция(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [CoatingMaterial](P_TFlex_Model_Model3D_Operation_CoatingMaterial.md) | Материал операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Color](P_TFlex_Model_Model3D_Object3D_Color.md) | Цвет(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ConstTransformations](P_TFlex_Model_Model3D_Object3D_ConstTransformations.md) | **Устарело.** Преобразование 3D объекта для чтения (устаревшая версия трансформации - допускается чтение трансформации в старых документах.)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Facet](P_TFlex_Model_Model3D_Operation_Facet.md) | (Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [FirstDegenerateProfile](P_TFlex_Model_Model3D_Loft_FirstDegenerateProfile.md) | Первый вырожденный профиль |
|  | [FirstDegenerateProfileCondition](P_TFlex_Model_Model3D_Loft_FirstDegenerateProfileCondition.md) | Граничное условие для первого вырожденного профиля, значение может быть равно 0 |
|  | [FirstEndProfileCondition](P_TFlex_Model_Model3D_Loft_FirstEndProfileCondition.md) | Cпециальное граничное условие для первого профиля, condition может быть равно 0 |
|  | [Fixed](P_TFlex_Model_Model3D_Operation_Fixed.md) | Свойство фиксации операции относительно сопряжений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Geometry](P_TFlex_Model_Model3D_Operation_Geometry.md) | Геометрические данные операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [GroupType](P_TFlex_Model_Model3D_Loft_GroupType.md) | Получить тип объекта(Переопределяет [OperationGroupType](P_TFlex_Model_Model3D_Operation_GroupType.md)) |
|  | [GuideAutoReverse](P_TFlex_Model_Model3D_Loft_GuideAutoReverse.md) | Автореверс для направляющих |
|  | [GuideCount](P_TFlex_Model_Model3D_Loft_GuideCount.md) | Получить число направляющих |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [InScene](P_TFlex_Model_Model3D_Object3D_InScene.md) | Объект в сцене(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTransparencyOn](P_TFlex_Model_Model3D_Operation_IsTransparencyOn.md) | Управление прозрачностью(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [KeepInitialSplitting](P_TFlex_Model_Model3D_Loft_KeepInitialSplitting.md) | Сохранять исходное разбиение |
|  | [LastDegenerateProfile](P_TFlex_Model_Model3D_Loft_LastDegenerateProfile.md) | Последний вырожденный профиль |
|  | [LastDegenerateProfileCondition](P_TFlex_Model_Model3D_Loft_LastDegenerateProfileCondition.md) | Граничное условие для последнего вырожденного профиля, значение может быть равно 0 |
|  | [LastEndProfileCondition](P_TFlex_Model_Model3D_Loft_LastEndProfileCondition.md) | Специальное граничное условие для последнего профиля, condition может быть равно 0 |
|  | [Layer](P_TFlex_Model_Model3D_Object3D_Layer.md) | Слой, на котором размещается объект(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Level](P_TFlex_Model_Model3D_Object3D_Level.md) | Уровень(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Linear](P_TFlex_Model_Model3D_Loft_Linear.md) | Линейчатая поверхность |
|  | [Material](P_TFlex_Model_Model3D_Operation_Material.md) | Материал операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MaterialDistributionLaw](P_TFlex_Model_Model3D_Operation_MaterialDistributionLaw.md) | (Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MeshDensity](P_TFlex_Model_Model3D_Operation_MeshDensity.md) | Плотность сетки в диапазоне 0.0-1.0(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Path](P_TFlex_Model_Model3D_Loft_Path.md) | Путь |
|  | [Periodic](P_TFlex_Model_Model3D_Loft_Periodic.md) | Периодическое построение лофтинга |
|  | [ProfileAutoReverse](P_TFlex_Model_Model3D_Loft_ProfileAutoReverse.md) | Автореверс для профилей |
|  | [ProfileCount](P_TFlex_Model_Model3D_Loft_ProfileCount.md) | Получить число профилей |
|  | [Suppression](P_TFlex_Model_Model3D_Operation_Suppression.md) | Свойство подавленности операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [ThinWall](P_TFlex_Model_Model3D_Loft_ThinWall.md) | Тонкостенное построение |
|  | [Tolerance](P_TFlex_Model_Model3D_Loft_Tolerance.md) | Точность |
|  | [TopLevel](P_TFlex_Model_Model3D_Operation_TopLevel.md) | Признак верхней операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [TopOperation](P_TFlex_Model_Model3D_Operation_TopOperation.md) | Верхняя операция в теле(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Transformations](P_TFlex_Model_Model3D_Object3D_Transformations.md) | Контейнер групп преобразований 3D объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Transparency](P_TFlex_Model_Model3D_Operation_Transparency.md) | Прозрачность(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [VisibleInScene](P_TFlex_Model_Model3D_Object3D_VisibleInScene.md) | Свойство видимости объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [VolatileTransformations](P_TFlex_Model_Model3D_Object3D_VolatileTransformations.md) | **Устарело.** Преобразование 3D объекта для изменения(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Wireframe](P_TFlex_Model_Model3D_Operation_Wireframe.md) | Признак рёберной отрисовки операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddGuide](M_TFlex_Model_Model3D_Loft_AddGuide.md) | Добавить направляющую |
|  | [AddGuideContour](M_TFlex_Model_Model3D_Loft_AddGuideContour.md) | Добавить контур к направляющей |
|  | [AddGuideFaceCondition](M_TFlex_Model_Model3D_Loft_AddGuideFaceCondition.md) | Добавить условие касания с гранью |
|  | [AddGuideVectorCondition](M_TFlex_Model_Model3D_Loft_AddGuideVectorCondition.md) | Добавить векторное условие на направляющей |
|  | [AddProfile](M_TFlex_Model_Model3D_Loft_AddProfile.md) | Добавить профиль |
|  | [AddProfileContour](M_TFlex_Model_Model3D_Loft_AddProfileContour.md) | Добавить контур к профилю |
|  | [AddProfileFaceCondition](M_TFlex_Model_Model3D_Loft_AddProfileFaceCondition.md) | Добавить условие касания с гранью |
|  | [AddProfileVectorCondition](M_TFlex_Model_Model3D_Loft_AddProfileVectorCondition.md) | Добавить векторное условие на профиле |
|  | [CancelRollback](M_TFlex_Model_Model3D_Object3D_CancelRollback.md) | Завершить откат(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CanSetAutomaticCouplingPoint](M_TFlex_Model_Model3D_Loft_CanSetAutomaticCouplingPoint.md) | Узнать можно ли установить автоматические точки соответствия |
|  | [CanSetPeriodic](M_TFlex_Model_Model3D_Loft_CanSetPeriodic.md) | Узнать можно ли установить параметр периодичности |
|  | [CanSetProfileFacesG2Condition](M_TFlex_Model_Model3D_Loft_CanSetProfileFacesG2Condition.md) | Узнать можно ли установить параметр взятия 2-й производной с граней |
|  | [Clone](M_TFlex_Model_Model3D_Object3D_Clone.md) | Класс для передачи ссылки на геометрические свойства родительского объекта или на отдельные геометрические элементы тел модели (грани, циклы, рёбра, вершины)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ConvertAutomaticCouplingPoints](M_TFlex_Model_Model3D_Loft_ConvertAutomaticCouplingPoints.md) | Конвертировать автоматические точки соответствия в типы PointVertex и PointEdge |
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
|  | [GetCouplingPoint](M_TFlex_Model_Model3D_Loft_GetCouplingPoint.md) | Задать точку соответствия |
|  | [GetCouplingPointVectorCondition](M_TFlex_Model_Model3D_Loft_GetCouplingPointVectorCondition.md) | Получить векторное условие на направляющей |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetGeomReference(Int32)](M_TFlex_Model_Model3D_Object3D_GetGeomReference.md) | Получить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetGeomReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_GetGeomReference_1.md) | Получить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetGuideContour](M_TFlex_Model_Model3D_Loft_GetGuideContour.md) | Возвращает контур направляющей |
|  | [GetGuideContourCount](M_TFlex_Model_Model3D_Loft_GetGuideContourCount.md) | Возвращает число контуров направляющей |
|  | [GetGuideFaceCondition](M_TFlex_Model_Model3D_Loft_GetGuideFaceCondition.md) | Получить условие касания с гранью |
|  | [GetGuideFaceConditionCount](M_TFlex_Model_Model3D_Loft_GetGuideFaceConditionCount.md) | Получить число условий касаний с гранью |
|  | [GetGuideReverse](M_TFlex_Model_Model3D_Loft_GetGuideReverse.md) | Возвращает реверс направляющей |
|  | [GetGuideVectorCondition](M_TFlex_Model_Model3D_Loft_GetGuideVectorCondition.md) | Получить векторное условие на направляющей |
|  | [GetGuideVectorConditionCount](M_TFlex_Model_Model3D_Loft_GetGuideVectorConditionCount.md) | Получить число векторных условий |
|  | [GetGuideVectorScaleFlag](M_TFlex_Model_Model3D_Loft_GetGuideVectorScaleFlag.md) | Возвращает параметр интерпретации коэффициента касательного вектора |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetProfileContour](M_TFlex_Model_Model3D_Loft_GetProfileContour.md) | Возвращает контур профиля |
|  | [GetProfileContourCount](M_TFlex_Model_Model3D_Loft_GetProfileContourCount.md) | Возвращает число контуров профиля |
|  | [GetProfileFaceCondition](M_TFlex_Model_Model3D_Loft_GetProfileFaceCondition.md) | Получить условие касания с гранью |
|  | [GetProfileFaceConditionCount](M_TFlex_Model_Model3D_Loft_GetProfileFaceConditionCount.md) | Получить число условий касаний с гранью |
|  | [GetProfileFacesG2Condition](M_TFlex_Model_Model3D_Loft_GetProfileFacesG2Condition.md) | Получить условие взятия 2-й производной с граней |
|  | [GetProfileReverse](M_TFlex_Model_Model3D_Loft_GetProfileReverse.md) | Возвращает реверс профиля |
|  | [GetProfileVectorCondition](M_TFlex_Model_Model3D_Loft_GetProfileVectorCondition.md) | Получить векторное условие на профиле |
|  | [GetProfileVectorConditionCount](M_TFlex_Model_Model3D_Loft_GetProfileVectorConditionCount.md) | Получить число векторных условий |
|  | [GetProfileVectorScaleFlag](M_TFlex_Model_Model3D_Loft_GetProfileVectorScaleFlag.md) | Возвращает параметр интерпретации коэффициента касательного вектора |
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
|  | [InsertCoupling](M_TFlex_Model_Model3D_Loft_InsertCoupling.md) | Вставить последовательность точек соответсвия |
|  | [InsertGuide](M_TFlex_Model_Model3D_Loft_InsertGuide.md) | Вставить направляющую в список направляющих |
|  | [InsertProfile](M_TFlex_Model_Model3D_Loft_InsertProfile.md) | Вставить профиль в список профилей |
|  | [InternalRegenerate](M_TFlex_Model_Model3D_Object3D_InternalRegenerate.md) | (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsAutomaticCouplingPointsSet](M_TFlex_Model_Model3D_Loft_IsAutomaticCouplingPointsSet.md) | Получить параметр автоматических точек соответствия |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [LockMateTransformation](M_TFlex_Model_Model3D_Operation_LockMateTransformation.md) | Заблокировать текущее преобразование сопряжений от дальнейших изменений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RemoveAllCouplingPointVectors](M_TFlex_Model_Model3D_Loft_RemoveAllCouplingPointVectors.md) | Удаляет все векторные условия в точках соответствия |
|  | [RemoveAllGuideContours](M_TFlex_Model_Model3D_Loft_RemoveAllGuideContours.md) | Удалить все контуры направляющей |
|  | [RemoveAllGuideFaceConditions](M_TFlex_Model_Model3D_Loft_RemoveAllGuideFaceConditions.md) | Удаляет все условия касания с гранью |
|  | [RemoveAllGuideVectorConditions](M_TFlex_Model_Model3D_Loft_RemoveAllGuideVectorConditions.md) | Удаляет все векторные условия |
|  | [RemoveAllProfileContours](M_TFlex_Model_Model3D_Loft_RemoveAllProfileContours.md) | Удалить все контуры профиля |
|  | [RemoveAllProfileFaceConditions](M_TFlex_Model_Model3D_Loft_RemoveAllProfileFaceConditions.md) | Удаляет все условия касания с гранью |
|  | [RemoveAllProfileVectorConditions](M_TFlex_Model_Model3D_Loft_RemoveAllProfileVectorConditions.md) | Удаляет все векторные условия |
|  | [RemoveCoupling](M_TFlex_Model_Model3D_Loft_RemoveCoupling.md) | Удалить последовательность точек соответсвия |
|  | [RemoveGuide](M_TFlex_Model_Model3D_Loft_RemoveGuide.md) | Удалить направляющую из списка направляющих |
|  | [RemoveGuideContour](M_TFlex_Model_Model3D_Loft_RemoveGuideContour.md) | Удалить контур направляющей |
|  | [RemoveProfile](M_TFlex_Model_Model3D_Loft_RemoveProfile.md) | Удалить профиль из списка профилей |
|  | [RemoveProfileContour](M_TFlex_Model_Model3D_Loft_RemoveProfileContour.md) | Удалить контур профиля |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ResetCouplingPoint](M_TFlex_Model_Model3D_Loft_ResetCouplingPoint.md) | Задать точку соответствия |
|  | [RollbackToParents](M_TFlex_Model_Model3D_Object3D_RollbackToParents.md) | Откат модели к состоянию, когда из сцены выгружены потомки объекта и он сам(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetAutomaticCouplingPoint](M_TFlex_Model_Model3D_Loft_SetAutomaticCouplingPoint.md) | Установить автоматические точки соответствия |
|  | [SetCouplingPoint](M_TFlex_Model_Model3D_Loft_SetCouplingPoint.md) | Задать точку соответствия |
|  | [SetCouplingPointVector](M_TFlex_Model_Model3D_Loft_SetCouplingPointVector.md) | Задать векторное условие в точке соответствия |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetGeomReference(Int32, Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_SetGeomReference.md) | Установить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetGeomReference(Int32, Object3DGeomReference, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_SetGeomReference_1.md) | Установить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetGuideReverse](M_TFlex_Model_Model3D_Loft_SetGuideReverse.md) | Установить реверс направляющей |
|  | [SetGuideVectorScaleFlag](M_TFlex_Model_Model3D_Loft_SetGuideVectorScaleFlag.md) | Устанавливает параметр использования коэффициента касательного вектора как масштабного |
|  | [SetProfileFacesG2Condition](M_TFlex_Model_Model3D_Loft_SetProfileFacesG2Condition.md) | Установить условие взятия 2-й производной с граней |
|  | [SetProfileReverse](M_TFlex_Model_Model3D_Loft_SetProfileReverse.md) | Установить реверс профиля |
|  | [SetProfileVectorScaleFlag](M_TFlex_Model_Model3D_Loft_SetProfileVectorScaleFlag.md) | Устанавливает параметр использования коэффициента касательного вектора как масштабного |
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
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)