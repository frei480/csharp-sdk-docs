

Руководство по T-FLEX CAD Open API

# RichText - класс  
    
Базовый класс форматированного текста

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model2DObject2D](T_TFlex_Model_Model2D_Object2D.md) [TFlex.Model.Model2DText](T_TFlex_Model_Model2D_Text.md) TFlex.Model.Model2DRichText [TFlex.Model.Model2DBOMObject](T_TFlex_Model_Model2D_BOMObject.md) [TFlex.Model.Model2DMultilineText](T_TFlex_Model_Model2D_MultilineText.md) [TFlex.Model.Model2DParagraphText](T_TFlex_Model_Model2D_ParagraphText.md)

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class RichText : Text
```
```vb
Public MustInherit Class RichText
	Inherits Text
```
```cpp
public ref class RichText abstract : public Text
```


Тип RichText предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [AutoUpdate](P_TFlex_Model_Model2D_RichText_AutoUpdate.md) | Автоматический пересчёт текста при открытом блоке изменения текста |
|  | [BoundRect](P_TFlex_Model_Model2D_Object2D_BoundRect.md) | Получение координат прямоугольника, обрамляющего объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CharacterFormat](P_TFlex_Model_Model2D_RichText_CharacterFormat.md) | Формат одного символа, на котором находится курсор, или символов, находящихся в выделенном фрагменте, в зависимости от состояния выделения |
|  | [Color](P_TFlex_Model_Model2D_Text_Color.md) | Цвет объекта(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [CurrFractionScale](P_TFlex_Model_Model2D_RichText_CurrFractionScale.md) | Текущий масштаб высоты шрифта для дробей, используется при вставке новых дробей |
|  | [CurrIndexScale](P_TFlex_Model_Model2D_RichText_CurrIndexScale.md) | Текущий масштаб высоты шрифта для индексов, используется при вставке новых индексов |
|  | [CursorPosition](P_TFlex_Model_Model2D_RichText_CursorPosition.md) | Положение курсора в тексте |
|  | [DefaultCharacterFormat](P_TFlex_Model_Model2D_RichText_DefaultCharacterFormat.md) | Формат символов, используемый по умолчанию |
|  | [DefaultNumberFormat](P_TFlex_Model_Model2D_RichText_DefaultNumberFormat.md) | Формат символов нумерации, используемый по умолчанию |
|  | [DefaultParagraphFormat](P_TFlex_Model_Model2D_RichText_DefaultParagraphFormat.md) | Формат абзацев, используемый по умолчанию |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [FontStyle](P_TFlex_Model_Model2D_Text_FontStyle.md) | Стиль шрифта текста(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [GroupType](P_TFlex_Model_Model2D_Text_GroupType.md) | Тип объекта(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model2D_Text_Layer.md) | Слой, на котором размещается объект(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [Level](P_TFlex_Model_Model2D_Text_Level.md) | Уровень объекта(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Page](P_TFlex_Model_Model2D_Text_Page.md) | Страница, на которой размещается элемент(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ParagraphFormat](P_TFlex_Model_Model2D_RichText_ParagraphFormat.md) | Формат одного символа, на котором находится курсор, или символов, находящихся в выделенном фрагменте, в зависимости от состояния выделения |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Priority](P_TFlex_Model_Model2D_Text_Priority.md) | Приоритет объекта(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [ProductStructureFile](P_TFlex_Model_Model2D_RichText_ProductStructureFile.md) | Ссылка на документ состава изделия по которому создан текст, если текст является отчетом состава изделия |
|  | [ProductStructureId](P_TFlex_Model_Model2D_RichText_ProductStructureId.md) | ID состава изделия по которому создан текст, если текст является отчетом состава изделия |
|  | [ReportPrototypeFile](P_TFlex_Model_Model2D_RichText_ReportPrototypeFile.md) | Ссылка на документ прототип отчета, если текст является отчетом состава изделия |
|  | [ShowVariableNames](P_TFlex_Model_Model2D_RichText_ShowVariableNames.md) | Показать имена переменных |
|  | [SubType](P_TFlex_Model_Model2D_Text_SubType.md) | Подтип текста(Унаследован от [Text](T_TFlex_Model_Model2D_Text.md)) |
|  | [TableOnly](P_TFlex_Model_Model2D_RichText_TableOnly.md) | Запретить ввод текста вне таблицы |
|  | [TextLength](P_TFlex_Model_Model2D_RichText_TextLength.md) | Получение длины всего текста с начала до конца без учёта таблиц |
|  | [TextValue](P_TFlex_Model_Model2D_RichText_TextValue.md) | Получение текста, находящегося в заданном отрезке |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [BeginEdit](M_TFlex_Model_Model2D_RichText_BeginEdit.md) | Начало редактирования текста |
|  | [ClearAll](M_TFlex_Model_Model2D_RichText_ClearAll.md) | Очистка содержимого всего текста |
|  | [Clone](M_TFlex_Model_ModelObject_Clone.md) | Создаёт копию объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyToClipboard](M_TFlex_Model_Model2D_RichText_CopyToClipboard.md) | Копировать выделенный текст в буфер обмена |
|  | [CreateObject](M_TFlex_Model_Model2D_Object2D_CreateObject.md) | (Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateTable(TableCreationSettings)](M_TFlex_Model_Model2D_RichText_CreateTable_1.md) | Создание таблицы перед символом, на котором находится курсор |
|  | [CreateTable(TableCreationSettings, TableCellProperties)](M_TFlex_Model_Model2D_RichText_CreateTable_2.md) |  |
|  | [CreateTable(UInt32, TableCreationSettings)](M_TFlex_Model_Model2D_RichText_CreateTable.md) | Создание таблицы перед символом, заданным порядковым номером относительно начала текста |
|  | [Delete](M_TFlex_Model_Model2D_RichText_Delete.md) | Удаление выделенного фрагмента или символа, на котором находится курсор |
|  | [Delete(UInt32)](M_TFlex_Model_Model2D_RichText_Delete_1.md) | Удаление нескольких символов, начиная с того, на котором находится курсор |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Deselect](M_TFlex_Model_Model2D_RichText_Deselect.md) | Снятие выделения |
|  | [Draw](M_TFlex_Model_Model2D_Object2D_Draw.md) | Нарисовать объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [EditInModalWindow](M_TFlex_Model_Model2D_RichText_EditInModalWindow.md) | Редактировать текст в модальном диалоге |
|  | [EndEdit](M_TFlex_Model_Model2D_RichText_EndEdit.md) | Завершение редактирования текста |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ExportToExcel](M_TFlex_Model_Model2D_RichText_ExportToExcel.md) | Экспортировать текст в Excel |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetCursorInfo](M_TFlex_Model_Model2D_RichText_GetCursorInfo.md) | Получение параметров положения курсора в тексте |
|  | [GetDefaultFontSize](M_TFlex_Model_Model2D_RichText_GetDefaultFontSize.md) | Получение размера символов, используемого по умолчанию |
|  | [GetDistance](M_TFlex_Model_Model2D_Object2D_GetDistance.md) | Получение растояния до объекта(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFirstTable](M_TFlex_Model_Model2D_RichText_GetFirstTable.md) |  |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetNextTable](M_TFlex_Model_Model2D_RichText_GetNextTable.md) |  |
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
|  | [GetSelectedRtfText](M_TFlex_Model_Model2D_RichText_GetSelectedRtfText.md) | Получение выделенного текста в формате RTF |
|  | [GetSelectedText](M_TFlex_Model_Model2D_RichText_GetSelectedText.md) | Получение выделенного текста |
|  | [GetSelection](M_TFlex_Model_Model2D_RichText_GetSelection.md) | Получение границ выделенного фрагмента |
|  | [GetTableByIndex](M_TFlex_Model_Model2D_RichText_GetTableByIndex.md) | Получение таблицы по её порядковому номеру |
|  | [GetTablePosition](M_TFlex_Model_Model2D_RichText_GetTablePosition.md) | Получение порядкового номера символа, перед которым находится таблица, относительно начала текста |
|  | [GetText](M_TFlex_Model_Model2D_RichText_GetText.md) | Получение текста, находящегося в заданном отрезке |
|  | [GetTextProp](M_TFlex_Model_ModelObject_GetTextProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProperty](M_TFlex_Model_ModelObject_GetTextProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InsertCommonSymbol](M_TFlex_Model_Model2D_RichText_InsertCommonSymbol.md) | Вставка символа |
|  | [InsertCopyOfTable(Table)](M_TFlex_Model_Model2D_RichText_InsertCopyOfTable_1.md) | Вставка копии таблицы перед символом, на котором находится курсор |
|  | [InsertCopyOfTable(UInt32, Table)](M_TFlex_Model_Model2D_RichText_InsertCopyOfTable.md) | Вставка копии таблицы перед символом, заданным порядковым номером относительно начала текста |
|  | [InsertFormLimitsSymbol](M_TFlex_Model_Model2D_RichText_InsertFormLimitsSymbol.md) | Вставка обозначения базы или допуска формы или расположения |
|  | [InsertFraction](M_TFlex_Model_Model2D_RichText_InsertFraction.md) | Вставка дроби |
|  | [InsertFragment](M_TFlex_Model_Model2D_RichText_InsertFragment.md) | Вставка фрагмента с указанием ссылки |
|  | [InsertFragment(FileLink)](M_TFlex_Model_Model2D_RichText_InsertFragment_1.md) | Вставка фрагмента с указанием ссылки |
|  | [InsertFragment(Fragment)](M_TFlex_Model_Model2D_RichText_InsertFragment_3.md) | **Устарело.** Вставка фрагмента |
|  | [InsertFragment(FileLink, RichTextInsertObjectOptions)](M_TFlex_Model_Model2D_RichText_InsertFragment_2.md) | Вставка фрагмента с указанием ссылки |
|  | [InsertHyperlink](M_TFlex_Model_Model2D_RichText_InsertHyperlink.md) | Вставка гиперссылки |
|  | [InsertImage](M_TFlex_Model_Model2D_RichText_InsertImage.md) | Вставка изображения с указанием ссылки |
|  | [InsertImage(FileLink)](M_TFlex_Model_Model2D_RichText_InsertImage_1.md) | Вставка изображения с указанием ссылки |
|  | [InsertImage(FileLink, RichTextInsertObjectOptions)](M_TFlex_Model_Model2D_RichText_InsertImage_2.md) | Вставка изображения с указанием ссылки |
|  | [InsertIndex](M_TFlex_Model_Model2D_RichText_InsertIndex.md) | Вставка индексов |
|  | [InsertParagraph](M_TFlex_Model_Model2D_RichText_InsertParagraph.md) | Вставка абзаца |
|  | [InsertParagraph(CharFormat)](M_TFlex_Model_Model2D_RichText_InsertParagraph_1.md) | Вставка абзаца с использованием заданного формата символов |
|  | [InsertParagraphs(UInt32)](M_TFlex_Model_Model2D_RichText_InsertParagraphs.md) | Вставка нескольких абзацев с использованием для разделителя формата символов по умолчанию для разделителя |
|  | [InsertParagraphs(UInt32, CharFormat)](M_TFlex_Model_Model2D_RichText_InsertParagraphs_1.md) | Вставка нескольких абзацев с использованием для разделителя заданного формата символов |
|  | [InsertRoughnessSymbol](M_TFlex_Model_Model2D_RichText_InsertRoughnessSymbol.md) | Вставка обозначения шероховатости |
|  | [InsertSymbol](M_TFlex_Model_Model2D_RichText_InsertSymbol.md) | Вставка символа с заданным кодом |
|  | [InsertText(String)](M_TFlex_Model_Model2D_RichText_InsertText.md) | Вставка текста с использованием формата символов по умолчанию |
|  | [InsertText(String, CharFormat)](M_TFlex_Model_Model2D_RichText_InsertText_1.md) | Вставка текста с использованием заданного формата символов |
|  | [InsertText(String, CharFormat, ParaFormat)](M_TFlex_Model_Model2D_RichText_InsertText_2.md) | Вставка текста с использованием заданного формата символов |
|  | [InsertTextWithHyperlinks](M_TFlex_Model_Model2D_RichText_InsertTextWithHyperlinks.md) |  |
|  | [InsertVariable](M_TFlex_Model_Model2D_RichText_InsertVariable.md) | Вставка переменной |
|  | [InsetRtfText](M_TFlex_Model_Model2D_RichText_InsetRtfText.md) | Вставка текста в формате RTF |
|  | [InternalRegenerate](M_TFlex_Model_ModelObject_InternalRegenerate.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveCursor](M_TFlex_Model_Model2D_RichText_MoveCursor.md) | Перемещение курсора на несколько символов вперёд или назад |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PasteFromClipboard](M_TFlex_Model_Model2D_RichText_PasteFromClipboard.md) | Вставить текст из буфера обмена |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ReplaceAbsentFontNames](M_TFlex_Model_Model2D_RichText_ReplaceAbsentFontNames.md) | Заменяем отсутствующие в системе шрифты во всех элементах текста. |
|  | [ReplaceFontName](M_TFlex_Model_Model2D_RichText_ReplaceFontName.md) | Заменяем выбранный шрифт во всех элементах текста. |
|  | [SelectAll](M_TFlex_Model_Model2D_RichText_SelectAll.md) | Выделение всего текста |
|  | [SetCursor(PositionProperties)](M_TFlex_Model_Model2D_RichText_SetCursor.md) | Установка положения курсора в тексте |
|  | [SetCursor(PositionProperties, PositionTablePosition)](M_TFlex_Model_Model2D_RichText_SetCursor_1.md) | Установка положения курсора в ячейке таблицы |
|  | [SetDefaultFont(String, Double, UInt32, Boolean)](M_TFlex_Model_Model2D_RichText_SetDefaultFont.md) | Установка шрифта, используемого по умолчанию |
|  | [SetDefaultFont(String, Double, UInt32, Boolean, Boolean)](M_TFlex_Model_Model2D_RichText_SetDefaultFont_1.md) | Установка шрифта, используемого по умолчанию |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetSelection(Position)](M_TFlex_Model_Model2D_RichText_SetSelection.md) | Установка выделения фрагмента, находящегося между курсором и заданной позицией |
|  | [SetSelection(Position, Position)](M_TFlex_Model_Model2D_RichText_SetSelection_1.md) | Установка выделения фрагмента текста |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Transform](M_TFlex_Model_Model2D_Object2D_Transform.md) | Применение преобразования.(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Translate](M_TFlex_Model_Model2D_Object2D_Translate.md) | Сдвиг объекта на данный вектор(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [TrySetTableOnly](M_TFlex_Model_Model2D_RichText_TrySetTableOnly.md) | Попробовать выставить свойство TableOnly |
  
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