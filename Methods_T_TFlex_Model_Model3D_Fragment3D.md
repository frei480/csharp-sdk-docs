

Руководство по T-FLEX CAD Open API

# Fragment3D - методы  
  
---  
  
Тип [Fragment3D](T_TFlex_Model_Model3D_Fragment3D.md) предоставляет следующие члены.

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
  
#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)