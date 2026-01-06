

Руководство по T-FLEX CAD Open API

# Fragment3D - класс  
    
Класс операции 3D фрагмента

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model3DObject3D](T_TFlex_Model_Model3D_Object3D.md) [TFlex.Model.Model3DOperation](T_TFlex_Model_Model3D_Operation.md) TFlex.Model.Model3DFragment3D

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Fragment3D : Operation
```
```vb
<ExtensionAttribute>
Public Class Fragment3D
	Inherits Operation
```
```cpp
[ExtensionAttribute]
public ref class Fragment3D : public Operation
```


Тип Fragment3D предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Fragment3D(FileLink)](M_TFlex_Model_Model3D_Fragment3D__ctor_2.md) | Конструктор с именем файла фрагмента |
|  | [Fragment3D(Fragment, Workplane)](M_TFlex_Model_Model3D_Fragment3D__ctor_3.md) | Конструктор с именем файла фрагмента |
|  | [Fragment3D(String, Document)](M_TFlex_Model_Model3D_Fragment3D__ctor.md) | Конструктор для создания 3D фрагмента |
|  | [Fragment3D(String, Document, Boolean, Boolean)](M_TFlex_Model_Model3D_Fragment3D__ctor_1.md) | Конструктор для создания 3D фрагмента |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Associative](P_TFlex_Model_Model3D_Fragment3D_Associative.md) |  |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [AttributesFromSource](P_TFlex_Model_Model3D_Fragment3D_AttributesFromSource.md) | Значение свойства "Атрибуты с исходной операции" |
|  | [AutoSave](P_TFlex_Model_Model3D_Fragment3D_AutoSave.md) | Создавать фрагмент в режиме автосохранения |
|  | [Auxiliary](P_TFlex_Model_Model3D_Object3D_Auxiliary.md) | Внутрисистемный объект. Используется для Refer объектов фрагментов. Такие объекты скрыты от пользователя. Работа с такими объектами может быть реализована на уровне API.NET или ядром TFlex. Такие объекты не передаются на следующий уровень сборки. (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Body](P_TFlex_Model_Model3D_Operation_Body.md) | Тело, в которое входит операция(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [BooleanOperationName](P_TFlex_Model_Model3D_Fragment3D_BooleanOperationName.md) | Имя операция для булевой операции |
|  | [CoatingMaterial](P_TFlex_Model_Model3D_Operation_CoatingMaterial.md) | Материал операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Color](P_TFlex_Model_Model3D_Object3D_Color.md) | Цвет(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Configuration](P_TFlex_Model_Model3D_Fragment3D_Configuration.md) | Имя конфигурации модели |
|  | [ConstTransformations](P_TFlex_Model_Model3D_Object3D_ConstTransformations.md) | **Устарело.** Преобразование 3D объекта для чтения (устаревшая версия трансформации - допускается чтение трансформации в старых документах.)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Facet](P_TFlex_Model_Model3D_Operation_Facet.md) | (Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [FileLink](P_TFlex_Model_Model3D_Fragment3D_FileLink.md) | Ссылка на файл фрагмента |
|  | [FileName](P_TFlex_Model_Model3D_Fragment3D_FileName.md) | **Устарело.** |
|  | [FilePath](P_TFlex_Model_Model3D_Fragment3D_FilePath.md) | Имя файла 3D Фрагмента |
|  | [Fixed](P_TFlex_Model_Model3D_Operation_Fixed.md) | Свойство фиксации операции относительно сопряжений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Fixing](P_TFlex_Model_Model3D_Fragment3D_Fixing.md) | Cпособ привязки 3D Фрагмента |
|  | [FragmentFileFolder](P_TFlex_Model_Model3D_Fragment3D_FragmentFileFolder.md) | Путь на папку относительно папки сборки при сохранении в папку сборки |
|  | [FreedomPropertyContainer](P_TFlex_Model_Model3D_Fragment3D_FreedomPropertyContainer.md) | Cтепени свободы 3D фрагмента |
|  | [FullFilePath](P_TFlex_Model_Model3D_Fragment3D_FullFilePath.md) | Полный путь файла 3D Фрагмента |
|  | [Geometry](P_TFlex_Model_Model3D_Operation_Geometry.md) | Геометрические данные операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [GroupType](P_TFlex_Model_Model3D_Fragment3D_GroupType.md) | Получить тип объекта(Переопределяет [OperationGroupType](P_TFlex_Model_Model3D_Operation_GroupType.md)) |
|  | [HideConnectors](P_TFlex_Model_Model3D_Fragment3D_HideConnectors.md) | Скрывать коннекторы |
|  | [HideLCSinTree](P_TFlex_Model_Model3D_Fragment3D_HideLCSinTree.md) | Не показывать системы координат в дереве модели |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IncludeInNewBom](P_TFlex_Model_Model3D_Fragment3D_IncludeInNewBom.md) | Включение в новую спецификацию |
|  | [IncludeInSpecificBom](P_TFlex_Model_Model3D_Fragment3D_IncludeInSpecificBom.md) | Включение в спецификацию |
|  | [InScene](P_TFlex_Model_Model3D_Object3D_InScene.md) | Объект в сцене(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [InverseTransformation](P_TFlex_Model_Model3D_Fragment3D_InverseTransformation.md) | Матрица обратного преобразования |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTransparencyOn](P_TFlex_Model_Model3D_Operation_IsTransparencyOn.md) | Управление прозрачностью(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model3D_Object3D_Layer.md) | Слой, на котором размещается объект(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Level](P_TFlex_Model_Model3D_Object3D_Level.md) | Уровень(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [LinkedDocumentGuid](P_TFlex_Model_Model3D_Fragment3D_LinkedDocumentGuid.md) |  |
|  | [Material](P_TFlex_Model_Model3D_Operation_Material.md) | Материал операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MaterialDistributionLaw](P_TFlex_Model_Model3D_Operation_MaterialDistributionLaw.md) | (Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MeshDensity](P_TFlex_Model_Model3D_Operation_MeshDensity.md) | Плотность сетки в диапазоне 0.0-1.0(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MoveX](P_TFlex_Model_Model3D_Fragment3D_MoveX.md) | Перемещение вдоль оси X |
|  | [MoveY](P_TFlex_Model_Model3D_Fragment3D_MoveY.md) | Перемещение вдоль оси Y |
|  | [MoveZ](P_TFlex_Model_Model3D_Fragment3D_MoveZ.md) | Перемещение вдоль оси Z |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parameters](P_TFlex_Model_Model3D_Fragment3D_Parameters.md) | Список идентификаторов объектов-параметров в документе фрагмента и объектов-значений в документе сборки |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PathName](P_TFlex_Model_Model3D_Fragment3D_PathName.md) | **Устарело.** |
|  | [Processing](P_TFlex_Model_Model3D_Fragment3D_Processing.md) | Обработка(Обогащение) фрагмента |
|  | [Reference](P_TFlex_Model_Model3D_Fragment3D_Reference.md) | Множество ссылочных объектов из которых состоит 3D Фрагмент |
|  | [RemoveAssociative](P_TFlex_Model_Model3D_Fragment3D_RemoveAssociative.md) | Разрывать ассоциативные связи при удалении объекта-значения параметра |
|  | [RotateX](P_TFlex_Model_Model3D_Fragment3D_RotateX.md) | Вращение по оси X |
|  | [RotateY](P_TFlex_Model_Model3D_Fragment3D_RotateY.md) | Вращение по оси Y |
|  | [RotateZ](P_TFlex_Model_Model3D_Fragment3D_RotateZ.md) | Вращение по оси Z |
|  | [SaveFragmentToAssemblyFolder](P_TFlex_Model_Model3D_Fragment3D_SaveFragmentToAssemblyFolder.md) | Cохранять файл фрагмента в папку сборки |
|  | [Separated](P_TFlex_Model_Model3D_Fragment3D_Separated.md) | Значение свойства "Как отдельные тела" |
|  | [ShowOn2D](P_TFlex_Model_Model3D_Fragment3D_ShowOn2D.md) | Показывать ли на 2D виде фрагмент |
|  | [SourceLCSName](P_TFlex_Model_Model3D_Fragment3D_SourceLCSName.md) | Имя системы координат созданной в документе фрагмента, используемой для привязки фрагмента |
|  | [Suppression](P_TFlex_Model_Model3D_Operation_Suppression.md) | Свойство подавленности операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [TargetLCS](P_TFlex_Model_Model3D_Fragment3D_TargetLCS.md) | Целевая система координат в документе сборки, используемая для привязки фрагмента |
|  | [TopLevel](P_TFlex_Model_Model3D_Operation_TopLevel.md) | Признак верхней операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [TopOperation](P_TFlex_Model_Model3D_Operation_TopOperation.md) | Верхняя операция в теле(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Transformations](P_TFlex_Model_Model3D_Object3D_Transformations.md) | Контейнер групп преобразований 3D объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Transparency](P_TFlex_Model_Model3D_Operation_Transparency.md) | Прозрачность(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [UseColorFromSource](P_TFlex_Model_Model3D_Fragment3D_UseColorFromSource.md) | Использовать цвет из документа фрагмента |
|  | [UseFragmentStatus](P_TFlex_Model_Model3D_Fragment3D_UseFragmentStatus.md) | Использовать статус документа фрагмента |
|  | [VariableValues](P_TFlex_Model_Model3D_Fragment3D_VariableValues.md) | **Устарело.** |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [VisibleInScene](P_TFlex_Model_Model3D_Object3D_VisibleInScene.md) | Свойство видимости объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [VolatileTransformations](P_TFlex_Model_Model3D_Object3D_VolatileTransformations.md) | **Устарело.** Преобразование 3D объекта для изменения(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Wireframe](P_TFlex_Model_Model3D_Operation_Wireframe.md) | Признак рёберной отрисовки операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Workplane](P_TFlex_Model_Model3D_Fragment3D_Workplane.md) | Рабочая плоскость, используемая для привязки фрагмента |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CancelRollback](M_TFlex_Model_Model3D_Object3D_CancelRollback.md) | Завершить откат(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ClearUDF](M_TFlex_Model_Model3D_Fragment3D_ClearUDF.md) | Удаление параметров адаптивного фрагмента |
|  | [Clone](M_TFlex_Model_Model3D_Object3D_Clone.md) | Класс для передачи ссылки на геометрические свойства родительского объекта или на отдельные геометрические элементы тел модели (грани, циклы, рёбра, вершины)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_Model3D_Fragment3D_Complete.md) | (Переопределяет [ModelObjectComplete](M_TFlex_Model_ModelObject_Complete.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateReference](M_TFlex_Model_Model3D_Object3D_CreateReference.md) | Создаёт ссылочный элемент в исходном документе(внутренняя ссылка)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CreateReference(Document)](M_TFlex_Model_Model3D_Object3D_CreateReference_1.md) | Создаёт ссылочный элемент в указанном документе(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DeleteMateTransformation](M_TFlex_Model_Model3D_Operation_DeleteMateTransformation.md) | Удалить текущее преобразование сопряжений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [EditAssocParams](M_TFlex_Model_Model3D_Fragment3D_EditAssocParams.md) | Редактирование параметров адаптивного фрагмента |
|  | [EditInContext](M_TFlex_Model_Model3D_Fragment3D_EditInContext.md) | Редактировать в контексте сборки |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ExportGeometry](M_TFlex_Model_Model3D_Operation_ExportGeometry.md) | Сохранение тел в файл в формате Parasolid(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindAssociatedFragment](M_TFlex_Model_Model3D_Fragment3D_FindAssociatedFragment.md) |  |
|  | [FindAssociatedTopols(Hole)](M_TFlex_Model_Model3D_Operation_FindAssociatedTopols.md) | Поиск топологических элементов, ассоциированных с отверстием(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [FindAssociatedTopols(LCS)](M_TFlex_Model_Model3D_Operation_FindAssociatedTopols_1.md) | Поиск топологических элементов, ассоциированных с системой координат(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [FindBodyOwner](M_TFlex_Model_Model3D_Operation_FindBodyOwner.md) | Получить базовую операцию, в которой хранятся свойства тела(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [FixByFragmentLCS](M_TFlex_Model_Model3D_Fragment3D_FixByFragmentLCS.md) | Привязать фрагмент по системе координат, существующей в документе фрагмента к системе координат в сборке |
|  | [FixByFragmentLCSToConnector](M_TFlex_Model_Model3D_Fragment3D_FixByFragmentLCSToConnector.md) | Привязать фрагмент по системе координат, существующей в документе фрагмента к системе координат в сборке. Если целевая система координат является коннектором, то выполняется связывание параметров. |
|  | [FixByWorkplane](M_TFlex_Model_Model3D_Fragment3D_FixByWorkplane.md) | Привязать фрагмент по расположению соответствующего 2D фрагмента на Рабочей плоскости |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetBOMQuantity](M_TFlex_Model_Model3D_Fragment3D_GetBOMQuantity.md) | Получить количество копий фрагмента во всех массивах |
|  | [GetDefaultLCS](M_TFlex_Model_Model3D_Fragment3D_GetDefaultLCS.md) | Имя системы координат, которая используется по умолчанию |
|  | [GetElevableLCS](M_TFlex_Model_Model3D_Fragment3D_GetElevableLCS.md) | Список систем координат, которые могут использоваться для привязки |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFragmentDocument(Boolean)](M_TFlex_Model_Model3D_Fragment3D_GetFragmentDocument.md) | Получить документ фрамента с подстановкой значений переменных фрагмента |
|  | [GetFragmentDocument(Boolean, Boolean)](M_TFlex_Model_Model3D_Fragment3D_GetFragmentDocument_1.md) | Получить документ фрамента с подстановкой значений переменных фрагмента |
|  | [GetGeomReference(Int32)](M_TFlex_Model_Model3D_Object3D_GetGeomReference.md) | Получить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetGeomReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_GetGeomReference_1.md) | Получить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetObjectFromFragment](M_TFlex_Model_Model3D_Fragment3D_GetObjectFromFragment.md) |  |
|  | [GetOperationToBoolean](M_TFlex_Model_Model3D_Fragment3D_GetOperationToBoolean.md) |  |
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
|  | [GetUserBomData](M_TFlex_Model_Model3D_Fragment3D_GetUserBomData.md) | Пользовательские данные для спецификации |
|  | [GetVariables](M_TFlex_Model_Model3D_Fragment3D_GetVariables.md) | Контейнер переменных фрагмента |
|  | [GetVariablesFromFragment](M_TFlex_Model_Model3D_Fragment3D_GetVariablesFromFragment.md) | Установить значения всех переменных фрагмента в соответствии с переменными входящего фрагмента |
|  | [GetVariableValue(String, Boolean)](M_TFlex_Model_Model3D_Fragment3D_GetVariableValue.md) | Получить переменную фрагмента по имени |
|  | [GetVariableValue(String, Boolean, Boolean)](M_TFlex_Model_Model3D_Fragment3D_GetVariableValue_1.md) | Получить переменную фрагмента по имени |
|  | [InternalRegenerate](M_TFlex_Model_Model3D_Object3D_InternalRegenerate.md) | (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [LockMateTransformation](M_TFlex_Model_Model3D_Operation_LockMateTransformation.md) | Заблокировать текущее преобразование сопряжений от дальнейших изменений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MakeParameters](M_TFlex_Model_Model3D_Fragment3D_MakeParameters.md) |  |
|  | [MarkChanged](M_TFlex_Model_Model3D_Fragment3D_MarkChanged.md) | Пометить объект как изменённый(Переопределяет [ModelObjectMarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCancelChanges](M_TFlex_Model_Model3D_Fragment3D_OnCancelChanges.md) | (Переопределяет [ModelObjectOnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md)) |
|  | [OnEndChanges](M_TFlex_Model_Model3D_Fragment3D_OnEndChanges.md) | (Переопределяет [ModelObjectOnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md)) |
|  | [OpenPart](M_TFlex_Model_Model3D_Fragment3D_OpenPart.md) | Создать деталировку |
|  | [OpenPart(FragmentOpenPartOptions)](M_TFlex_Model_Model3D_Fragment3D_OpenPart_1.md) | Создать деталировку с данными параметрами |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RememberTopLabel](M_TFlex_Model_Model3D_Fragment3D_RememberTopLabel.md) | Запомнить метку верхушки Undo-стэка |
|  | [RemoveParameters](M_TFlex_Model_Model3D_Fragment3D_RemoveParameters.md) |  |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RollbackToParents](M_TFlex_Model_Model3D_Object3D_RollbackToParents.md) | Откат модели к состоянию, когда из сцены выгружены потомки объекта и он сам(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetGeomReference(Int32, Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_SetGeomReference.md) | Установить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetGeomReference(Int32, Object3DGeomReference, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_SetGeomReference_1.md) | Установить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_Model3D_Object3D_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetUniqueName](M_TFlex_Model_Model3D_Object3D_SetUniqueName.md) | Установить новое уникальное имя с заданным префиксом(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ShowVariablesDialog](M_TFlex_Model_Model3D_Fragment3D_ShowVariablesDialog.md) | Показать диалог "Переменные" |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [UpdateDetail](M_TFlex_Model_Model3D_Fragment3D_UpdateDetail.md) | Обновить деталь |
|  | [UpdateVariablesFromFragmentDocument](M_TFlex_Model_Model3D_Fragment3D_UpdateVariablesFromFragmentDocument.md) | Обновить все переменные фрагмента по документу фрагмента |
|  | [UpdateVariablesFromFragmentDocument(Boolean)](M_TFlex_Model_Model3D_Fragment3D_UpdateVariablesFromFragmentDocument_1.md) | Обновить переменные фрагмента по документу фрагмента |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_AddMultilineText.md) | Аггрегировать новый многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineText.md) | Получить аггрегированный многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextBounds](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextBounds.md) | Получить габариты аггрегированного многострочного текста(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextsCount](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextsCount.md) | Количество аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [RemoveMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_RemoveMultilineText.md) | Удалить многострочный текст по индексу(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [UpdateMultilineTextPage](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_UpdateMultilineTextPage.md) | Обновить страницу аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
      
    
    public static void FragmentLCS(string pathFragment, PointsLCS lcs)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");
    
       Fragment3D fr = new Fragment3D(pathFragment, document);
       fr.FixByFragmentLCS(lcs.Name, lcs); //привязка фрагмента к системе координат(название системы координат, сама система)
    
       document.EndChanges();//Закрытие блока изменений документа
    }
    
    
    public static void FragmentVariables(string pathFragment)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");
    
       Fragment3D fragment = new Fragment3D(pathFragment, document);
       foreach(FragmentVariableValue v in fragment.GetVariables())//цикл по переменным фрагмента
       {
        if(v.Name == "D" && v.IsReal)//находим переменную "D" 
        {
            v.RealValue = 100;//устанавливаем значение
        }
       }
    
       document.EndChanges();//Закрытие блока изменений документа
    }
    
    
    public static void FragmentOpenPart(string pathFragment)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");
    
       Fragment3D fr = new Fragment3D(pathFragment, document);
       fr.OpenPart(); //деталировка
    
       document.EndChanges();//Закрытие блока изменений документа
    }
    
    
    public static void FragmentMethodPlan(WorkPlane onPointsWorkplane, string pathFragment)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");
    
       Fragment f = new Fragment(document, pathFragment);//2D-фрагмент, имеющий 3D реализацию
       f.Page = onPointsWorkplane.Page;//привязка фрагмента к странице плоскости
       Fragment3D fr = new Fragment3D(f, onPointsWorkplane);//3D-фрагмент на основе 2D-фрагмента и плоскости
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)