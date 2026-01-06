

Руководство по T-FLEX CAD Open API

# Fragment - класс  
    
Класс 2D фрагмента

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model2DObject2D](T_TFlex_Model_Model2D_Object2D.md) TFlex.Model.Model2DFragment

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class Fragment : Object2D, IModelObjectWithLayer
```
```vb
Public Class Fragment
	Inherits Object2D
	Implements IModelObjectWithLayer
```
```cpp
public ref class Fragment : public Object2D, 
	IModelObjectWithLayer
```


Тип Fragment предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Fragment(Document)](M_TFlex_Model_Model2D_Fragment__ctor.md) | Конструктор по умолчанию |
|  | [Fragment(FileLink)](M_TFlex_Model_Model2D_Fragment__ctor_3.md) | Конструктор с именем файла фрагмента |
|  | [Fragment(Document, String)](M_TFlex_Model_Model2D_Fragment__ctor_1.md) | Конструктор с именем файла фрагмента |
|  | [Fragment(Document, String, Boolean, Boolean)](M_TFlex_Model_Model2D_Fragment__ctor_2.md) | Конструктор с именем файла фрагмента |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AlwaysRegenerate3DModel](P_TFlex_Model_Model2D_Fragment_AlwaysRegenerate3DModel.md) | Всегда пересчитывать 3D модель |
|  | [Angle](P_TFlex_Model_Model2D_Fragment_Angle.md) | Угол поворота вектора привязки |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [AutoSave](P_TFlex_Model_Model2D_Fragment_AutoSave.md) | Создавать фрагмент в режиме автосохранения |
|  | [BoundRect](P_TFlex_Model_Model2D_Object2D_BoundRect.md) | Получение координат прямоугольника, обрамляющего объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CanDraw](P_TFlex_Model_Model2D_Fragment_CanDraw.md) |  |
|  | [Connector](P_TFlex_Model_Model2D_Fragment_Connector.md) | Коннектор, к которому привязан фрагмент |
|  | [Constant](P_TFlex_Model_Model2D_Fragment_Constant.md) | Параметр "Постоянный фрагмент (символ)" |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [EndNode](P_TFlex_Model_Model2D_Fragment_EndNode.md) | Узел привязки конечной точки вектора привязки |
|  | [EndX](P_TFlex_Model_Model2D_Fragment_EndX.md) | Координата X привязки конечной точки вектора привязки |
|  | [EndY](P_TFlex_Model_Model2D_Fragment_EndY.md) | Координата Y привязки конечной точки вектора привязки |
|  | [FileLink](P_TFlex_Model_Model2D_Fragment_FileLink.md) | Ссылка на файл фрагмента |
|  | [FilePath](P_TFlex_Model_Model2D_Fragment_FilePath.md) | Имя файла фрагмента |
|  | [FragmentDocumentPage](P_TFlex_Model_Model2D_Fragment_FragmentDocumentPage.md) | Страница с которой берётся фрагмент |
|  | [FragmentFileFolder](P_TFlex_Model_Model2D_Fragment_FragmentFileFolder.md) | Путь на папку относительно папки сборки при сохранении в папку сборки |
|  | [FullFilePath](P_TFlex_Model_Model2D_Fragment_FullFilePath.md) | Полный путь файла фрагмента |
|  | [GroupType](P_TFlex_Model_Model2D_Fragment_GroupType.md) | Тип объекта(Переопределяет [ModelObjectGroupType](P_TFlex_Model_ModelObject_GroupType.md)) |
|  | [HasAssociatedFragment](P_TFlex_Model_Model2D_Fragment_HasAssociatedFragment.md) |  |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IncludeInNewBom](P_TFlex_Model_Model2D_Fragment_IncludeInNewBom.md) | Включение в новую спецификацию |
|  | [IncludeInSpecificBom](P_TFlex_Model_Model2D_Fragment_IncludeInSpecificBom.md) | Включение в спецификацию |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model2D_Fragment_Layer.md) | Слой, на котором размещается объект |
|  | [Level](P_TFlex_Model_Model2D_Fragment_Level.md) | Уровень объекта |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Page](P_TFlex_Model_Model2D_Fragment_Page.md) | Страница, на которой размещается элемент(Переопределяет [Object2DPage](P_TFlex_Model_Model2D_Object2D_Page.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Priority](P_TFlex_Model_Model2D_Fragment_Priority.md) | Приоритет объекта |
|  | [SaveFragmentToAssemblyFolder](P_TFlex_Model_Model2D_Fragment_SaveFragmentToAssemblyFolder.md) | Cохранять файл фрагмента в папку сборки |
|  | [Scale](P_TFlex_Model_Model2D_Fragment_Scale.md) | Параметр "Масштаб" |
|  | [ScaleLineWidth](P_TFlex_Model_Model2D_Fragment_ScaleLineWidth.md) | Параметр "Масштабировать толщину линий" |
|  | [StartNode](P_TFlex_Model_Model2D_Fragment_StartNode.md) | Узел привязки начальной точки вектора привязки |
|  | [StartX](P_TFlex_Model_Model2D_Fragment_StartX.md) | Координата X привязки начальной точки вектора привязки |
|  | [StartY](P_TFlex_Model_Model2D_Fragment_StartY.md) | Координата Y привязки начальной точки вектора привязки |
|  | [Symmetric](P_TFlex_Model_Model2D_Fragment_Symmetric.md) | Параметр "Симметричный относительно вектора привязки" |
|  | [Transformation](P_TFlex_Model_Model2D_Fragment_Transformation.md) | Получить текущее преобразование фрагмента |
|  | [UseAssemblyStatus](P_TFlex_Model_Model2D_Fragment_UseAssemblyStatus.md) | Использовать статус сборки, иначе - статус документа фрагмента |
|  | [VariableValues](P_TFlex_Model_Model2D_Fragment_VariableValues.md) | **Устарело.** |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AssignAssemblyVariables](M_TFlex_Model_Model2D_Fragment_AssignAssemblyVariables.md) | Назначить переменные сборки по умолчанию |
|  | [Clone](M_TFlex_Model_ModelObject_Clone.md) | Создаёт копию объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Create3DFragment](M_TFlex_Model_Model2D_Fragment_Create3DFragment.md) | Создать 3D фрагмент |
|  | [CreateObject](M_TFlex_Model_Model2D_Object2D_CreateObject.md) | (Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Draw](M_TFlex_Model_Model2D_Object2D_Draw.md) | Нарисовать объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [EditInContext](M_TFlex_Model_Model2D_Fragment_EditInContext.md) | Редактировать в контексте сборки |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Explode(Boolean)](M_TFlex_Model_Model2D_Fragment_Explode.md) | Раскрыть фрагмент |
|  | [Explode(FragmentExplodeOptions)](M_TFlex_Model_Model2D_Fragment_Explode_1.md) | Раскрыть фрагмент |
|  | [ExtractFragment](M_TFlex_Model_Model2D_Fragment_ExtractFragment.md) | Создание фрагмента на основе списка объектов (Выделить фрагмент) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetBOMQuantity](M_TFlex_Model_Model2D_Fragment_GetBOMQuantity.md) | Получить количество копий фрагмента в всех массивах |
|  | [GetDeepVariable](M_TFlex_Model_Model2D_Fragment_GetDeepVariable.md) |  |
|  | [GetDistance](M_TFlex_Model_Model2D_Object2D_GetDistance.md) | Получение растояния до объекта(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFixingNode](M_TFlex_Model_Model2D_Fragment_GetFixingNode.md) | Установка узла привязки точки привязки фрагмента, привязанного при помощи переменных привязки |
|  | [GetFixingVectorCount](M_TFlex_Model_Model2D_Fragment_GetFixingVectorCount.md) | Получить количество векторов привязки фрагмента |
|  | [GetFixingVectorName](M_TFlex_Model_Model2D_Fragment_GetFixingVectorName.md) | Получить имя текущего вектора привязки фрагмента |
|  | [GetFixingVectorName(Int32)](M_TFlex_Model_Model2D_Fragment_GetFixingVectorName_1.md) | Получить имя вектора привязки фрагмента с указанным номером |
|  | [GetFixingX](M_TFlex_Model_Model2D_Fragment_GetFixingX.md) | Получение координаты X точки привязки фрагмента, привязанного при помощи переменных привязки |
|  | [GetFixingY](M_TFlex_Model_Model2D_Fragment_GetFixingY.md) | Получение координаты Y точки привязки фрагмента, привязанного при помощи переменных привязки |
|  | [GetFragmentDocument](M_TFlex_Model_Model2D_Fragment_GetFragmentDocument.md) | Получить документ фрамента |
|  | [GetFragmentDocument(Boolean)](M_TFlex_Model_Model2D_Fragment_GetFragmentDocument_1.md) | Получить документ фрамента с подстановкой значений переменных фрагмента |
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
|  | [GetUserBomData](M_TFlex_Model_Model2D_Fragment_GetUserBomData.md) | Пользовательские данные для спецификации |
|  | [GetVariables](M_TFlex_Model_Model2D_Fragment_GetVariables.md) | Контейнер переменных фрагмента |
|  | [GetVariables(Boolean)](M_TFlex_Model_Model2D_Fragment_GetVariables_1.md) | Получить контейнер переменных фрагмента |
|  | [GetVariables(Boolean, Boolean)](M_TFlex_Model_Model2D_Fragment_GetVariables_2.md) | Контейнер переменных фрагмента |
|  | [GetVariablesFromFragment](M_TFlex_Model_Model2D_Fragment_GetVariablesFromFragment.md) | Установить значения всех переменных фрагмента в соответствии с переменными входящего фрагмента |
|  | [GetVariableValue(String, Boolean)](M_TFlex_Model_Model2D_Fragment_GetVariableValue.md) | Получить переменную фрагмента по имени |
|  | [GetVariableValue(String, Boolean, Boolean)](M_TFlex_Model_Model2D_Fragment_GetVariableValue_1.md) | Получить переменную фрагмента по имени |
|  | [HaveFixingPoint](M_TFlex_Model_Model2D_Fragment_HaveFixingPoint.md) | Проверка существования точки привязки фрагмента, привязанного при помощи переменных привязки |
|  | [HideAssociatedLayers](M_TFlex_Model_Model2D_Fragment_HideAssociatedLayers.md) | Гасим слои, связанные с вектором привязки |
|  | [HideAssociatedLayers(Document)](M_TFlex_Model_Model2D_Fragment_HideAssociatedLayers_1.md) | Гасим слои, связанные с вектором привязки |
|  | [InternalRegenerate](M_TFlex_Model_ModelObject_InternalRegenerate.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OpenPart](M_TFlex_Model_Model2D_Fragment_OpenPart.md) | Создать деталировку |
|  | [OpenPart(FragmentOpenPartOptions)](M_TFlex_Model_Model2D_Fragment_OpenPart_1.md) | Создать деталировку с данными параметрами |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RestoreAssociatedLayers](M_TFlex_Model_Model2D_Fragment_RestoreAssociatedLayers.md) | Восстанавливаем видимость слоев, связанных с вектором привязки |
|  | [RestoreAssociatedLayers(Document)](M_TFlex_Model_Model2D_Fragment_RestoreAssociatedLayers_1.md) | Восстанавливаем видимость слоев, связанных с вектором привязки |
|  | [SetDefaultFixingVector](M_TFlex_Model_Model2D_Fragment_SetDefaultFixingVector.md) | Установить привязку фрагмента по основному вектору привязки |
|  | [SetDefaultVariableValues](M_TFlex_Model_Model2D_Fragment_SetDefaultVariableValues.md) | Установить значения переменных фрагмента из документа фрагмента |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFixingNode](M_TFlex_Model_Model2D_Fragment_SetFixingNode.md) | Установка узла привязки точки привязки фрагмента, привязанного при помощи переменных привязки |
|  | [SetFixingPoint](M_TFlex_Model_Model2D_Fragment_SetFixingPoint.md) | Установка координат точки привязки фрагмента, привязанного при помощи переменных привязки |
|  | [SetFixingVectorName](M_TFlex_Model_Model2D_Fragment_SetFixingVectorName.md) | Установить привязку фрагмента по вектору привязки с указанным именем |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ShowVariablesDialog](M_TFlex_Model_Model2D_Fragment_ShowVariablesDialog.md) | Показать диалог "Переменные" |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Transform](M_TFlex_Model_Model2D_Object2D_Transform.md) | Применение преобразования.(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Translate](M_TFlex_Model_Model2D_Object2D_Translate.md) | Сдвиг объекта на данный вектор(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [UpdateVariablesFromFragmentDocument](M_TFlex_Model_Model2D_Fragment_UpdateVariablesFromFragmentDocument.md) | Обновить переменные фрагмента по документу фрагмента |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_AddMultilineText.md) | Аггрегировать новый многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [FindAssociatedFragment](M_TFlex_Model_Model3D_Fragment3D_FindAssociatedFragment.md) | (Определяется [Fragment3D](T_TFlex_Model_Model3D_Fragment3D.md)) |
|  | [GetMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineText.md) | Получить аггрегированный многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextBounds](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextBounds.md) | Получить габариты аггрегированного многострочного текста(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextsCount](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextsCount.md) | Количество аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [RemoveMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_RemoveMultilineText.md) | Удалить многострочный текст по индексу(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [UpdateMultilineTextPage](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_UpdateMultilineTextPage.md) | Обновить страницу аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
      
    
    public static void FragmentNodes(string pathFragment)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа            
       document.BeginChanges("2D фрагменты вставка по узлам");//Открытие блока изменений документа
    
       Fragment fragment = new Fragment(document, pathFragment);//фрагмент
       FreeNode fn1 = new FreeNode(document, 0, 180);
       fragment.SetFixingNode(1, fn1);//Установка узла привязки точки привязки фрагмента, привязанного при помощи переменных привязки
    
       document.EndChanges();//Закрытие блока изменений документа
    }
    
    
    public static void FragmentFixingVector(string pathFragment)
    {    
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("2D фрагменты вставка по вектору привязки");//Открытие блока изменений документа
    
       Fragment fragment = new Fragment(document, pathFragment);            
       FixingVector fv = new FixingVector(document); //вектор привязки
       fv.Name = "FixingVector";
    
       FreeNode fn1 = new FreeNode(document, 10, 160);
       FreeNode fn2 = new FreeNode(document, 100, 160);
    
       fv.StartNode = fn1;
       fv.EndNode = fn2;
       fv.Color = 200;
       //установить привязку фрагмента по вектору привязки с указанным именем
       fragment.SetFixingVectorName("FixingVector");
    
       document.EndChanges();//Закрытие блока изменений документа
    }
    
    
    public static void FragmentConnector(string pathFragment)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("2D фрагменты вставка по коннектору");//Открытие блока изменений документа
    
       Fragment fragment = new Fragment(document, pathFragment);//фрагмент    
       FreeNode fn1 = new FreeNode(document, -100, 700);
       fragment.SetFixingNode(1, fn1);
       Connector connector = new Connector(document);//коннектор
       connector.StartNode = new FreeNode(document, -100, 700);//Начальный узел            
       connector.EndNode = new FreeNode(document, 100, 700);//Конечный узел            
       fragment.Connector = connector;//привязка созданного коннектора к фрагменту
    
       document.EndChanges();//Закрытие блока изменений документа
    }
    
    
    public static void FragmentVariables(string pathFragment)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("2D фрагменты");//Открытие блока изменений документа
    
       Fragment fragment = new Fragment(document, pathFragment);
       foreach(FragmentVariableValue v in fragment.GetVariables())//цикл по переменным фрагмента
       {
        if(v.Name == "D" && v.IsReal)//находим переменную "D" 
        {
            v.RealValue = 100;//устанавливаем значение
        }
       }
    
       document.EndChanges();//Закрытие блока изменений документа
    }
    
    
    public static void FragmentAction(string pathFragment)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("действия над фрагментами");//Открытие блока изменений документа
    
       Fragment fragment = new Fragment(document, pathFragment);
       fragment.EditInContext();//Редактировать в контексте сборки
       fragment.Explode(true);//Раскрыть фрагмент true - с построением
       fragment.OpenPart();//деталировка
    
       document.EndChanges();//Закрытие блока изменений документа            
    }

#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)