

Руководство по T-FLEX CAD Open API

# BOMObject - класс  
    
Класс спецификации

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model2DObject2D](T_TFlex_Model_Model2D_Object2D.md) [TFlex.Model.Model2DText](T_TFlex_Model_Model2D_Text.md) [TFlex.Model.Model2DRichText](T_TFlex_Model_Model2D_RichText.md) TFlex.Model.Model2DBOMObject

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class BOMObject : RichText
```
```vb
Public Class BOMObject
	Inherits RichText
```
```cpp
public ref class BOMObject : public RichText
```


Тип BOMObject предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [AutoUpdate](P_TFlex_Model_Model2D_RichText_AutoUpdate.md) | Автоматический пересчёт текста при открытом блоке изменения текста(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [BoundRect](P_TFlex_Model_Model2D_Object2D_BoundRect.md) | Получение координат прямоугольника, обрамляющего объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CharacterFormat](P_TFlex_Model_Model2D_RichText_CharacterFormat.md) | Формат одного символа, на котором находится курсор, или символов, находящихся в выделенном фрагменте, в зависимости от состояния выделения(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [Color](P_TFlex_Model_Model2D_Text_Color.md) | Цвет объекта(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [CurrFractionScale](P_TFlex_Model_Model2D_RichText_CurrFractionScale.md) | Текущий масштаб высоты шрифта для дробей, используется при вставке новых дробей(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [CurrIndexScale](P_TFlex_Model_Model2D_RichText_CurrIndexScale.md) | Текущий масштаб высоты шрифта для индексов, используется при вставке новых индексов(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [CursorPosition](P_TFlex_Model_Model2D_RichText_CursorPosition.md) | Положение курсора в тексте(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [DefaultCharacterFormat](P_TFlex_Model_Model2D_RichText_DefaultCharacterFormat.md) | Формат символов, используемый по умолчанию(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [DefaultNumberFormat](P_TFlex_Model_Model2D_RichText_DefaultNumberFormat.md) | Формат символов нумерации, используемый по умолчанию(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [DefaultParagraphFormat](P_TFlex_Model_Model2D_RichText_DefaultParagraphFormat.md) | Формат абзацев, используемый по умолчанию(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [FontStyle](P_TFlex_Model_Model2D_Text_FontStyle.md) | Стиль шрифта текста(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [FriendlyName](P_TFlex_Model_Model2D_BOMObject_FriendlyName.md) | Название спецификации |
|  | [GroupType](P_TFlex_Model_Model2D_Text_GroupType.md) | Тип объекта(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsUsedForSetupPositions](P_TFlex_Model_Model2D_BOMObject_IsUsedForSetupPositions.md) | Используется для простановки позиций |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model2D_Text_Layer.md) | Слой, на котором размещается объект(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [Level](P_TFlex_Model_Model2D_Text_Level.md) | Уровень объекта(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [LinkedFragment](P_TFlex_Model_Model2D_BOMObject_LinkedFragment.md) | Связанный фрагмент |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [NewGroupUseMaxPosition](P_TFlex_Model_Model2D_BOMObject_NewGroupUseMaxPosition.md) | Начинать нумерацию в разделе после максимального значения в предыдущем разделе |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Page](P_TFlex_Model_Model2D_Text_Page.md) | Страница, на которой размещается элемент(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ParagraphFormat](P_TFlex_Model_Model2D_RichText_ParagraphFormat.md) | Формат одного символа, на котором находится курсор, или символов, находящихся в выделенном фрагменте, в зависимости от состояния выделения(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Priority](P_TFlex_Model_Model2D_Text_Priority.md) | Приоритет объекта(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [ProductStructureFile](P_TFlex_Model_Model2D_RichText_ProductStructureFile.md) | Ссылка на документ состава изделия по которому создан текст, если текст является отчетом состава изделия(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [ProductStructureId](P_TFlex_Model_Model2D_RichText_ProductStructureId.md) | ID состава изделия по которому создан текст, если текст является отчетом состава изделия(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [RecordFlags](P_TFlex_Model_Model2D_BOMObject_RecordFlags.md) | Флаги состояния текущей записи |
|  | [RecordGroup](P_TFlex_Model_Model2D_BOMObject_RecordGroup.md) | Номер раздела текущей записи |
|  | [RecordGroupFullName](P_TFlex_Model_Model2D_BOMObject_RecordGroupFullName.md) | Полное имя раздела текущей записи |
|  | [RecordID](P_TFlex_Model_Model2D_BOMObject_RecordID.md) | ID текущей записи |
|  | [RecordPosition](P_TFlex_Model_Model2D_BOMObject_RecordPosition.md) | Номер позиции текущей записи |
|  | [RecordSpaceAfter](P_TFlex_Model_Model2D_BOMObject_RecordSpaceAfter.md) | Пропуск строк после текущей записи |
|  | [RecordSpaceBefore](P_TFlex_Model_Model2D_BOMObject_RecordSpaceBefore.md) | Пропуск строк перед текущей записью |
|  | [RecordVersion](P_TFlex_Model_Model2D_BOMObject_RecordVersion.md) | Номер исполнения текущей записи |
|  | [ReportFileLink](P_TFlex_Model_Model2D_BOMObject_ReportFileLink.md) | Ссылка на документ спецификации |
|  | [ReportID](P_TFlex_Model_Model2D_BOMObject_ReportID.md) | Идентификатор связаного объекта в документе спецификации |
|  | [ReportPrototypeFile](P_TFlex_Model_Model2D_RichText_ReportPrototypeFile.md) | Ссылка на документ прототип отчета, если текст является отчетом состава изделия(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [ShowVariableNames](P_TFlex_Model_Model2D_RichText_ShowVariableNames.md) | Показать имена переменных(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SortByPosition](P_TFlex_Model_Model2D_BOMObject_SortByPosition.md) | Сортировка по позициям |
|  | [SubType](P_TFlex_Model_Model2D_BOMObject_SubType.md) | Подтип спецификации(Переопределяет [TextSubType](P_TFlex_Model_Model2D_Text_SubType.md)) |
|  | [TableOnly](P_TFlex_Model_Model2D_RichText_TableOnly.md) | Запретить ввод текста вне таблицы(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [TextLength](P_TFlex_Model_Model2D_RichText_TextLength.md) | Получение длины всего текста с начала до конца без учёта таблиц(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [TextValue](P_TFlex_Model_Model2D_RichText_TextValue.md) | Получение текста, находящегося в заданном отрезке(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddRecord](M_TFlex_Model_Model2D_BOMObject_AddRecord.md) | Добавить запись |
|  | [BeginEdit](M_TFlex_Model_Model2D_BOMObject_BeginEdit.md) | Начать изменение спецификации |
|  | [ClearAll](M_TFlex_Model_Model2D_RichText_ClearAll.md) | Очистка содержимого всего текста(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [Clone](M_TFlex_Model_ModelObject_Clone.md) | Создаёт копию объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyToClipboard](M_TFlex_Model_Model2D_RichText_CopyToClipboard.md) | Копировать выделенный текст в буфер обмена(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [CreateCustomColumn](M_TFlex_Model_Model2D_BOMObject_CreateCustomColumn.md) | Создать колонку пользовательского типа |
|  | [CreateField(String, BOMObjectFieldType)](M_TFlex_Model_Model2D_BOMObject_CreateField.md) | Создать поле |
|  | [CreateField(String, BOMObjectFiledType)](M_TFlex_Model_Model2D_BOMObject_CreateField_1.md) | **Устарело.** |
|  | [CreateObject](M_TFlex_Model_Model2D_Object2D_CreateObject.md) | (Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CreateStandardColumn](M_TFlex_Model_Model2D_BOMObject_CreateStandardColumn.md) | Создать колонку стандартного типа |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateTable(TableCreationSettings)](M_TFlex_Model_Model2D_RichText_CreateTable_1.md) | Создание таблицы перед символом, на котором находится курсор(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [CreateTable(TableCreationSettings, TableCellProperties)](M_TFlex_Model_Model2D_RichText_CreateTable_2.md) | (Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [CreateTable(UInt32, TableCreationSettings)](M_TFlex_Model_Model2D_RichText_CreateTable.md) | Создание таблицы перед символом, заданным порядковым номером относительно начала текста(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [CreateVariableColumn](M_TFlex_Model_Model2D_BOMObject_CreateVariableColumn.md) | Создать колонку переменного типа |
|  | [Delete](M_TFlex_Model_Model2D_RichText_Delete.md) | Удаление выделенного фрагмента или символа, на котором находится курсор(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [Delete(UInt32)](M_TFlex_Model_Model2D_RichText_Delete_1.md) | Удаление нескольких символов, начиная с того, на котором находится курсор(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [DeleteAllRecords](M_TFlex_Model_Model2D_BOMObject_DeleteAllRecords.md) | Удалить все записи |
|  | [DeleteRecord](M_TFlex_Model_Model2D_BOMObject_DeleteRecord.md) | Удалить текущую запись |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Deselect](M_TFlex_Model_Model2D_RichText_Deselect.md) | Снятие выделения(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [Draw](M_TFlex_Model_Model2D_Object2D_Draw.md) | Нарисовать объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [EditRecord](M_TFlex_Model_Model2D_BOMObject_EditRecord.md) | Редактировать текущую запись |
|  | [EndEdit](M_TFlex_Model_Model2D_BOMObject_EndEdit.md) | Завершить изменение спецификации |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ExportToExcel](M_TFlex_Model_Model2D_RichText_ExportToExcel.md) | Экспортировать текст в Excel(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAllFields](M_TFlex_Model_Model2D_BOMObject_GetAllFields.md) | Получить имена всех полей |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetBOMGroups](M_TFlex_Model_Model2D_BOMObject_GetBOMGroups.md) | Получить массив всех разделов спецификации |
|  | [GetCursorInfo](M_TFlex_Model_Model2D_RichText_GetCursorInfo.md) | Получение параметров положения курсора в тексте(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetDefaultFontSize](M_TFlex_Model_Model2D_RichText_GetDefaultFontSize.md) | Получение размера символов, используемого по умолчанию(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetDistance](M_TFlex_Model_Model2D_Object2D_GetDistance.md) | Получение растояния до объекта(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [GetFieldGuidValueIndirect](M_TFlex_Model_Model2D_BOMObject_GetFieldGuidValueIndirect.md) | Получить значение поля в виде GUID |
|  | [GetFieldIntValueIndirect](M_TFlex_Model_Model2D_BOMObject_GetFieldIntValueIndirect.md) | Получить целое значение поля |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFirstTable](M_TFlex_Model_Model2D_RichText_GetFirstTable.md) | (Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetNextTable](M_TFlex_Model_Model2D_RichText_GetNextTable.md) | (Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
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
|  | [GetSelectedRtfText](M_TFlex_Model_Model2D_RichText_GetSelectedRtfText.md) | Получение выделенного текста в формате RTF(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetSelectedText](M_TFlex_Model_Model2D_RichText_GetSelectedText.md) | Получение выделенного текста(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetSelection](M_TFlex_Model_Model2D_RichText_GetSelection.md) | Получение границ выделенного фрагмента(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetStandardFieldFlag](M_TFlex_Model_Model2D_BOMObject_GetStandardFieldFlag.md) |  |
|  | [GetStandardFieldValue](M_TFlex_Model_Model2D_BOMObject_GetStandardFieldValue.md) | Получить значение стандартного поля |
|  | [GetTableByIndex](M_TFlex_Model_Model2D_RichText_GetTableByIndex.md) | Получение таблицы по её порядковому номеру(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetTablePosition](M_TFlex_Model_Model2D_RichText_GetTablePosition.md) | Получение порядкового номера символа, перед которым находится таблица, относительно начала текста(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetText](M_TFlex_Model_Model2D_RichText_GetText.md) | Получение текста, находящегося в заданном отрезке(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [GetTextProp](M_TFlex_Model_ModelObject_GetTextProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProperty](M_TFlex_Model_ModelObject_GetTextProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetUserFieldValue](M_TFlex_Model_Model2D_BOMObject_GetUserFieldValue.md) | Получить значение пользовательского поля |
|  | [GetVisibleFields](M_TFlex_Model_Model2D_BOMObject_GetVisibleFields.md) | Получить имена видимых полей в порядке отображения |
|  | [InsertCommonSymbol](M_TFlex_Model_Model2D_RichText_InsertCommonSymbol.md) | Вставка символа(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertCopyOfTable(Table)](M_TFlex_Model_Model2D_RichText_InsertCopyOfTable_1.md) | Вставка копии таблицы перед символом, на котором находится курсор(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertCopyOfTable(UInt32, Table)](M_TFlex_Model_Model2D_RichText_InsertCopyOfTable.md) | Вставка копии таблицы перед символом, заданным порядковым номером относительно начала текста(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertFormLimitsSymbol](M_TFlex_Model_Model2D_RichText_InsertFormLimitsSymbol.md) | Вставка обозначения базы или допуска формы или расположения(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertFraction](M_TFlex_Model_Model2D_RichText_InsertFraction.md) | Вставка дроби(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertFragment](M_TFlex_Model_Model2D_RichText_InsertFragment.md) | Вставка фрагмента с указанием ссылки(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertFragment(FileLink)](M_TFlex_Model_Model2D_RichText_InsertFragment_1.md) | Вставка фрагмента с указанием ссылки(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertFragment(Fragment)](M_TFlex_Model_Model2D_RichText_InsertFragment_3.md) | **Устарело.** Вставка фрагмента(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertFragment(FileLink, RichTextInsertObjectOptions)](M_TFlex_Model_Model2D_RichText_InsertFragment_2.md) | Вставка фрагмента с указанием ссылки(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertHyperlink](M_TFlex_Model_Model2D_RichText_InsertHyperlink.md) | Вставка гиперссылки(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertImage](M_TFlex_Model_Model2D_RichText_InsertImage.md) | Вставка изображения с указанием ссылки(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertImage(FileLink)](M_TFlex_Model_Model2D_RichText_InsertImage_1.md) | Вставка изображения с указанием ссылки(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertImage(FileLink, RichTextInsertObjectOptions)](M_TFlex_Model_Model2D_RichText_InsertImage_2.md) | Вставка изображения с указанием ссылки(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertIndex](M_TFlex_Model_Model2D_RichText_InsertIndex.md) | Вставка индексов(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertParagraph](M_TFlex_Model_Model2D_RichText_InsertParagraph.md) | Вставка абзаца(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertParagraph(CharFormat)](M_TFlex_Model_Model2D_RichText_InsertParagraph_1.md) | Вставка абзаца с использованием заданного формата символов(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertParagraphs(UInt32)](M_TFlex_Model_Model2D_RichText_InsertParagraphs.md) | Вставка нескольких абзацев с использованием для разделителя формата символов по умолчанию для разделителя(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertParagraphs(UInt32, CharFormat)](M_TFlex_Model_Model2D_RichText_InsertParagraphs_1.md) | Вставка нескольких абзацев с использованием для разделителя заданного формата символов(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertRoughnessSymbol](M_TFlex_Model_Model2D_RichText_InsertRoughnessSymbol.md) | Вставка обозначения шероховатости(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertSymbol](M_TFlex_Model_Model2D_RichText_InsertSymbol.md) | Вставка символа с заданным кодом(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertText(String)](M_TFlex_Model_Model2D_RichText_InsertText.md) | Вставка текста с использованием формата символов по умолчанию(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertText(String, CharFormat)](M_TFlex_Model_Model2D_RichText_InsertText_1.md) | Вставка текста с использованием заданного формата символов(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertText(String, CharFormat, ParaFormat)](M_TFlex_Model_Model2D_RichText_InsertText_2.md) | Вставка текста с использованием заданного формата символов(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertTextWithHyperlinks](M_TFlex_Model_Model2D_RichText_InsertTextWithHyperlinks.md) | (Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsertVariable](M_TFlex_Model_Model2D_RichText_InsertVariable.md) | Вставка переменной(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InsetRtfText](M_TFlex_Model_Model2D_RichText_InsetRtfText.md) | Вставка текста в формате RTF(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [InternalRegenerate](M_TFlex_Model_ModelObject_InternalRegenerate.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveCursor](M_TFlex_Model_Model2D_RichText_MoveCursor.md) | Перемещение курсора на несколько символов вперёд или назад(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [MoveToFrontRecord](M_TFlex_Model_Model2D_BOMObject_MoveToFrontRecord.md) | Перевести курсор на первую запись спецификации |
|  | [MoveToNextRecord](M_TFlex_Model_Model2D_BOMObject_MoveToNextRecord.md) | Перевести курсор на следующую запись спецификации |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PasteFromClipboard](M_TFlex_Model_Model2D_RichText_PasteFromClipboard.md) | Вставить текст из буфера обмена(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Refresh](M_TFlex_Model_Model2D_BOMObject_Refresh.md) | Обновить спецификацию |
|  | [Refresh(Boolean)](M_TFlex_Model_Model2D_BOMObject_Refresh_1.md) | Обновить данные спецификации и спецификацию |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ReplaceAbsentFontNames](M_TFlex_Model_Model2D_RichText_ReplaceAbsentFontNames.md) | Заменяем отсутствующие в системе шрифты во всех элементах текста.(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [ReplaceFontName](M_TFlex_Model_Model2D_RichText_ReplaceFontName.md) | Заменяем выбранный шрифт во всех элементах текста.(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SeekToRecordID](M_TFlex_Model_Model2D_BOMObject_SeekToRecordID.md) | Перевести курсор на запись спецификации с заданным ID |
|  | [SelectAll](M_TFlex_Model_Model2D_RichText_SelectAll.md) | Выделение всего текста(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SetCursor(PositionProperties)](M_TFlex_Model_Model2D_RichText_SetCursor.md) | Установка положения курсора в тексте(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SetCursor(PositionProperties, PositionTablePosition)](M_TFlex_Model_Model2D_RichText_SetCursor_1.md) | Установка положения курсора в ячейке таблицы(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SetDefaultFont(String, Double, UInt32, Boolean)](M_TFlex_Model_Model2D_RichText_SetDefaultFont.md) | Установка шрифта, используемого по умолчанию(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SetDefaultFont(String, Double, UInt32, Boolean, Boolean)](M_TFlex_Model_Model2D_RichText_SetDefaultFont_1.md) | Установка шрифта, используемого по умолчанию(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SetFieldGuidValueIndirect](M_TFlex_Model_Model2D_BOMObject_SetFieldGuidValueIndirect.md) | Установить значение поля в виде GUID |
|  | [SetFieldIntValueIndirect](M_TFlex_Model_Model2D_BOMObject_SetFieldIntValueIndirect.md) | Установить целое значение поля |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetSelection(Position)](M_TFlex_Model_Model2D_RichText_SetSelection.md) | Установка выделения фрагмента, находящегося между курсором и заданной позицией(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SetSelection(Position, Position)](M_TFlex_Model_Model2D_RichText_SetSelection_1.md) | Установка выделения фрагмента текста(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [SetVersions](M_TFlex_Model_Model2D_BOMObject_SetVersions.md) | Установить исполнения |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Transform](M_TFlex_Model_Model2D_Object2D_Transform.md) | Применение преобразования.(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Translate](M_TFlex_Model_Model2D_Object2D_Translate.md) | Сдвиг объекта на данный вектор(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [TrySetTableOnly](M_TFlex_Model_Model2D_RichText_TrySetTableOnly.md) | Попробовать выставить свойство TableOnly(Унаследован от [RichText](T_TFlex_Model_Model2D_RichText.md)) |
|  | [UpdateRecord](M_TFlex_Model_Model2D_BOMObject_UpdateRecord.md) | Обновить текущую запись |
|  | [UpdateStandardFieldValue](M_TFlex_Model_Model2D_BOMObject_UpdateStandardFieldValue.md) | Установить значение стандартного поля |
|  | [UpdateUserFieldValue](M_TFlex_Model_Model2D_BOMObject_UpdateUserFieldValue.md) | Установить значение пользовательского поля |
  
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