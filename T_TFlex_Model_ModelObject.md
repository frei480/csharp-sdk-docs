

Руководство по T-FLEX CAD Open API

# ModelObject - класс  
  
---  
  
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelModelObject Подробнее

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class ModelObject : ICloneable, 
	IComparable
```
```vb
Public MustInherit Class ModelObject
	Implements ICloneable, IComparable
```
```cpp
public ref class ModelObject abstract : ICloneable, 
	IComparable
```


Тип ModelObject предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ModelObject](M_TFlex_Model_ModelObject__ctor.md) | Для внутреннего использования |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.** |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования |
|  | [GroupType](P_TFlex_Model_ModelObject_GroupType.md) | Идентификатор типа данного объекта |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'. |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_ModelObject_Clone.md) | Создаёт копию объекта |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) |  |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер |
|  | [CreateReferenceObject](M_TFlex_Model_ModelObject_CreateReferenceObject.md) |  |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) |  |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта |
|  | [GetProperties](M_TFlex_Model_ModelObject_GetProperties.md) | Получить описание свойств элемента |
|  | [GetRealProp](M_TFlex_Model_ModelObject_GetRealProp.md) | **Устарело.** Измеримые свойства объекта |
|  | [GetRealProperty](M_TFlex_Model_ModelObject_GetRealProperty.md) | Получить значение свойства элемента |
|  | [GetRealPropertyWithUnit](M_TFlex_Model_ModelObject_GetRealPropertyWithUnit.md) |  |
|  | [GetReference(Int32)](M_TFlex_Model_ModelObject_GetReference.md) | Получить ссылку на родительский объект по ключу |
|  | [GetReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetReference_1.md) | Получить ссылку на родительский объект по ключу и индексу. Используется для организации массивов |
|  | [GetReferences](M_TFlex_Model_ModelObject_GetReferences.md) |  |
|  | [GetRegenerationResult](M_TFlex_Model_ModelObject_GetRegenerationResult.md) | Результат пересчета объекта |
|  | [GetRelation](M_TFlex_Model_ModelObject_GetRelation.md) | Измерить отношение двух объектов |
|  | [GetRelationWithUnit](M_TFlex_Model_ModelObject_GetRelationWithUnit.md) |  |
|  | [GetTextProp](M_TFlex_Model_ModelObject_GetTextProp.md) | **Устарело.** Измеримые свойства объекта |
|  | [GetTextProperty](M_TFlex_Model_ModelObject_GetTextProperty.md) | Получить значение свойства элемента |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InternalRegenerate](M_TFlex_Model_ModelObject_InternalRegenerate.md) |  |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) |  |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый |
|  | [Measure(ObjectArray, ModelObject)](M_TFlex_Model_ModelObject_Measure_1.md) | Измерить все параметры одного объекта либо отношения нескольких объектов |
|  | [Measure(ObjectArray, String, ModelObject)](M_TFlex_Model_ModelObject_Measure.md) | Измерить параметр одного объекта либо отношение нескольких объектов |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) |  |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) |  |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов |
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

[TFlex.Model - пространство имён](N_TFlex_Model.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelModelObject [TFlex.ModelDatabase](T_TFlex_Model_Database.md) [TFlex.ModelLayer](T_TFlex_Model_Layer.md) [TFlex.Model.Model2DObject2D](T_TFlex_Model_Model2D_Object2D.md) [TFlex.Model.Model3DMaterial](T_TFlex_Model_Model3D_Material.md) [TFlex.Model.Model3DObject3D](T_TFlex_Model_Model3D_Object3D.md) [TFlex.Model.Model3DRestraint](T_TFlex_Model_Model3D_Restraint.md) [TFlex.Model.Model3DSensor](T_TFlex_Model_Model3D_Sensor.md) [TFlex.Model.Model3DStudy](T_TFlex_Model_Model3D_Study.md) [TFlex.Model.Model3DTransformation](T_TFlex_Model_Model3D_Transformation.md) [TFlex.ModelPage](T_TFlex_Model_Page.md) [TFlex.ModelProductStructure](T_TFlex_Model_ProductStructure.md) [TFlex.ModelRowElement](T_TFlex_Model_RowElement.md) [TFlex.Model.StructureElement](T_TFlex_Model_Structure_Element.md) [TFlex.Model.StructureElementLink](T_TFlex_Model_Structure_ElementLink.md) [TFlex.Model.StructureElementType](T_TFlex_Model_Structure_ElementType.md) [TFlex.Model.StructureLinkDescriptor](T_TFlex_Model_Structure_LinkDescriptor.md) [TFlex.ModelVariable](T_TFlex_Model_Variable.md) [TFlex.ModelWeld](T_TFlex_Model_Weld.md) [TFlex.ModelWeldType](T_TFlex_Model_WeldType.md)