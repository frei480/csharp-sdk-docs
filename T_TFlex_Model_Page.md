

Руководство по T-FLEX CAD Open API

# Page - класс  
  
---  
  
Класс страницы документа

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) TFlex.ModelPage

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class Page : ModelObject
```
```vb
Public NotInheritable Class Page
	Inherits ModelObject
```
```cpp
public ref class Page sealed : public ModelObject
```


Тип Page предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Page(Document)](M_TFlex_Model_Page__ctor.md) | Конструктор |
|  | [Page(Page)](M_TFlex_Model_Page__ctor_2.md) | Конструктор |
|  | [Page(Document, PageType)](M_TFlex_Model_Page__ctor_1.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AngularDimensionMinimalDigits](P_TFlex_Model_Page_AngularDimensionMinimalDigits.md) | Минимальное количество цифр после точки для угловых размеров |
|  | [AngularDimensionPrecision](P_TFlex_Model_Page_AngularDimensionPrecision.md) | Точность угловых размеров |
|  | [AngularDimensionUnits](P_TFlex_Model_Page_AngularDimensionUnits.md) | Единицы измерения угловых размеров |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Bottom](P_TFlex_Model_Page_Bottom.md) | Нижняя Y-координата границ бумаги |
|  | [DefaultArrowSize](P_TFlex_Model_Page_DefaultArrowSize.md) | Размер стрелок по умолчанию |
|  | [DegreeCode](P_TFlex_Model_Page_DegreeCode.md) | Код символа "градус" |
|  | [DiameterCode](P_TFlex_Model_Page_DiameterCode.md) | Код символа "диаметр" |
|  | [DimensionQuality](P_TFlex_Model_Page_DimensionQuality.md) | Квалитет размеров по умолчанию |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DrawingLimits](P_TFlex_Model_Page_DrawingLimits.md) | Прямоугольник границ элементов страницы |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [FontStyle](P_TFlex_Model_Page_FontStyle.md) | Стиль шрифта текста |
|  | [FragmentForNewPageFileLink](P_TFlex_Model_Page_FragmentForNewPageFileLink.md) | Ссылка на документ, который будет вставлен, как фрагмент, при создании страницы, следующей за этой страницей |
|  | [GroupType](P_TFlex_Model_Page_GroupType.md) | Идентификатор типа объекта(Переопределяет [ModelObjectGroupType](P_TFlex_Model_ModelObject_GroupType.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IndexSymbolScale](P_TFlex_Model_Page_IndexSymbolScale.md) | Масштаб подстрочных и надстрочных символов |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsSelectedForExporting](P_TFlex_Model_Page_IsSelectedForExporting.md) | Страница, выбранная для экспорта |
|  | [IsSelectedForPrinting](P_TFlex_Model_Page_IsSelectedForPrinting.md) | Страница, выбранная для печати |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Left](P_TFlex_Model_Page_Left.md) | Левая X-координата границ бумаги |
|  | [LinearDimensionMinimalDigits](P_TFlex_Model_Page_LinearDimensionMinimalDigits.md) | Минимальное количество цифр после точки для линейных размеров |
|  | [LinearDimensionPrecision](P_TFlex_Model_Page_LinearDimensionPrecision.md) | Точность линейных размеров |
|  | [LinearDimensionUnits](P_TFlex_Model_Page_LinearDimensionUnits.md) | Единицы измерения линейных размеров |
|  | [LinePatternScale](P_TFlex_Model_Page_LinePatternScale.md) | Масштаб штрихов штриховых линий по умолчанию |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_Page_Name.md) | Имя страницы(Переопределяет [ModelObjectName](P_TFlex_Model_ModelObject_Name.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PageType](P_TFlex_Model_Page_PageType.md) | Тип страницы |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PlusMinusCode](P_TFlex_Model_Page_PlusMinusCode.md) | Код символа "плюс-минус" |
|  | [Properties](P_TFlex_Model_Page_Properties.md) |  |
|  | [Rank](P_TFlex_Model_Page_Rank.md) | Порядковый номер страницы |
|  | [Rectangle](P_TFlex_Model_Page_Rectangle.md) | Прямоугольник границ страницы |
|  | [Right](P_TFlex_Model_Page_Right.md) | Правая X-координата границ бумаги |
|  | [Scale](P_TFlex_Model_Page_Scale.md) | Масштаб страницы |
|  | [SelectionMode](P_TFlex_Model_Page_SelectionMode.md) | Режим выбора элементов |
|  | [SymbolFontName](P_TFlex_Model_Page_SymbolFontName.md) | Имя символьного шрифта |
|  | [ThickLineThickness](P_TFlex_Model_Page_ThickLineThickness.md) | Толщина основных линий по умолчанию |
|  | [ThinLineThickness](P_TFlex_Model_Page_ThinLineThickness.md) | Толщина тонких линий по умолчанию |
|  | [Top](P_TFlex_Model_Page_Top.md) | Верхняя Y-координата границ бумаги |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_ModelObject_Clone.md) | Создаёт копию объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
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
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PrepareGraphics](M_TFlex_Model_Page_PrepareGraphics.md) | Подготовка графического контекста для прорисовки на данной странице |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ResetName](M_TFlex_Model_Page_ResetName.md) | Перезадать имя страницы согласно правилам именования страниц |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_AddMultilineText.md) | Аггрегировать новый многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineText.md) | Получить аггрегированный многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextBounds](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextBounds.md) | Получить габариты аггрегированного многострочного текста(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextsCount](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextsCount.md) | Количество аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [RemoveMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_RemoveMultilineText.md) | Удалить многострочный текст по индексу(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [UpdateMultilineTextPage](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_UpdateMultilineTextPage.md) | Обновить страницу аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
      
    
    public static void Page()//создания новой страницы и установки её параметров
    {            
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("Новая страница");//Открытие блока изменений документа
    
       Page p = new Page(document);
       p.Name = "Новая страница";//название страницы
       p.FontStyle.Italic = true;//устновка стиля шрифта - наклонный        
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)