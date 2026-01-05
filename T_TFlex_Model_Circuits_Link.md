

Руководство по T-FLEX CAD Open API

# Link - класс  
  
---  
  
Объект "линия связи"

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model2DObject2D](T_TFlex_Model_Model2D_Object2D.md) [TFlex.Model.CircuitsLinkBase](T_TFlex_Model_Circuits_LinkBase.md) TFlex.Model.CircuitsLink [TFlex.Model.CircuitsBus](T_TFlex_Model_Circuits_Bus.md) [TFlex.Model.CircuitsLinksGroup](T_TFlex_Model_Circuits_LinksGroup.md)

**Пространство имён:** [TFlex.Model.Circuits](N_TFlex_Model_Circuits.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class Link : LinkBase
```
```vb
Public Class Link
	Inherits LinkBase
```
```cpp
public ref class Link : public LinkBase
```


Тип Link предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [BoundRect](P_TFlex_Model_Model2D_Object2D_BoundRect.md) | Получение координат прямоугольника, обрамляющего объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CanDraw](P_TFlex_Model_Circuits_Link_CanDraw.md) | (Переопределяет [LinkBaseCanDraw](P_TFlex_Model_Circuits_LinkBase_CanDraw.md)) |
|  | [Coaxial](P_TFlex_Model_Circuits_Link_Coaxial.md) | Атрибуты линии связи |
|  | [Color](P_TFlex_Model_Circuits_Link_Color.md) | Цвет линии связи |
|  | [DashColor](P_TFlex_Model_Circuits_Link_DashColor.md) | Цвет штрихов линии связи |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GroupType](P_TFlex_Model_Circuits_Link_GroupType.md) | (Переопределяет [ModelObjectGroupType](P_TFlex_Model_ModelObject_GroupType.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Optical](P_TFlex_Model_Circuits_Link_Optical.md) |  |
|  | [Page](P_TFlex_Model_Circuits_Link_Page.md) | Страница, на которой размещается элемент(Переопределяет [Object2DPage](P_TFlex_Model_Model2D_Object2D_Page.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PartlyShielded](P_TFlex_Model_Circuits_Link_PartlyShielded.md) |  |
|  | [Shielded](P_TFlex_Model_Circuits_Link_Shielded.md) |  |
|  | [Splices](P_TFlex_Model_Circuits_LinkBase_Splices.md) | (Унаследован от [LinkBase](T_TFlex_Model_Circuits_LinkBase.md)) |
|  | [TextOffset](P_TFlex_Model_Circuits_Link_TextOffset.md) | (Переопределяет [LinkBaseTextOffset](P_TFlex_Model_Circuits_LinkBase_TextOffset.md)) |
|  | [TwistedPair](P_TFlex_Model_Circuits_Link_TwistedPair.md) |  |
|  | [Type](P_TFlex_Model_Circuits_Link_Type.md) | Тип линии связи |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDesignation(String, String, DesignationType)](M_TFlex_Model_Circuits_Link_AddDesignation.md) | (Переопределяет [LinkBaseAddDesignation(String, String, DesignationType)](M_TFlex_Model_Circuits_LinkBase_AddDesignation.md)) |
|  | [AddDesignation(String, String, DesignationType, String)](M_TFlex_Model_Circuits_Link_AddDesignation_1.md) | (Переопределяет [LinkBaseAddDesignation(String, String, DesignationType, String)](M_TFlex_Model_Circuits_LinkBase_AddDesignation_1.md)) |
|  | [AddDesignation(String, FixingVector, Double, String, DesignationType)](M_TFlex_Model_Circuits_Link_AddDesignation_2.md) | (Переопределяет [LinkBaseAddDesignation(String, FixingVector, Double, String, DesignationType)](M_TFlex_Model_Circuits_LinkBase_AddDesignation_2.md)) |
|  | [AddWireConnectionInfo](M_TFlex_Model_Circuits_Link_AddWireConnectionInfo.md) | (Переопределяет [LinkBaseAddWireConnectionInfo(Element, ModelObject, ModelObject)](M_TFlex_Model_Circuits_LinkBase_AddWireConnectionInfo.md)) |
|  | [CanInsert(FixingVector)](M_TFlex_Model_Circuits_Link_CanInsert.md) | Проверка, можно ли вставить point в линию |
|  | [CanInsert(FixingVector, FixingVector)](M_TFlex_Model_Circuits_Link_CanInsert_1.md) | Проверка, можно ли вставить point1 и point2 в линию |
|  | [Clone](M_TFlex_Model_ModelObject_Clone.md) | Создаёт копию объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_ModelObject_Complete.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Create](M_TFlex_Model_Circuits_Link_Create.md) |  |
|  | [CreateObject](M_TFlex_Model_Model2D_Object2D_CreateObject.md) | (Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Draw](M_TFlex_Model_Model2D_Object2D_Draw.md) | Нарисовать объект(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAllLinkedObjects](M_TFlex_Model_Circuits_Link_GetAllLinkedObjects.md) | (Переопределяет [LinkBaseGetAllLinkedObjects](M_TFlex_Model_Circuits_LinkBase_GetAllLinkedObjects.md)) |
|  | [GetAllWireConnectionInfos](M_TFlex_Model_Circuits_Link_GetAllWireConnectionInfos.md) | (Переопределяет [LinkBaseGetAllWireConnectionInfos(Boolean)](M_TFlex_Model_Circuits_LinkBase_GetAllWireConnectionInfos.md)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetDesignations](M_TFlex_Model_Circuits_Link_GetDesignations.md) | (Переопределяет [LinkBaseGetDesignations(DesignationType)](M_TFlex_Model_Circuits_LinkBase_GetDesignations.md)) |
|  | [GetDistance](M_TFlex_Model_Model2D_Object2D_GetDistance.md) | Получение растояния до объекта(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFontOptions](M_TFlex_Model_Circuits_Link_GetFontOptions.md) | (Переопределяет [LinkBaseGetFontOptions](M_TFlex_Model_Circuits_LinkBase_GetFontOptions.md)) |
|  | [GetFreePoints](M_TFlex_Model_Circuits_Link_GetFreePoints.md) | Координаты точек, которые ни к чему не подключены |
|  | [GetGroups](M_TFlex_Model_Circuits_Link_GetGroups.md) | (Переопределяет [LinkBaseGetGroups](M_TFlex_Model_Circuits_LinkBase_GetGroups.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetLinkPoint](M_TFlex_Model_Circuits_Link_GetLinkPoint.md) | (Переопределяет [LinkBaseGetLinkPoint(FixingVector)](M_TFlex_Model_Circuits_LinkBase_GetLinkPoint.md)) |
|  | [GetLinksGroup](M_TFlex_Model_Circuits_Link_GetLinksGroup.md) |  |
|  | [GetMultiLink](M_TFlex_Model_Circuits_Link_GetMultiLink.md) | Получить линию связи с разрывом |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetNearestPoint](M_TFlex_Model_Circuits_Link_GetNearestPoint.md) |  |
|  | [GetPathBoundRect](M_TFlex_Model_Circuits_Link_GetPathBoundRect.md) | (Переопределяет [LinkBaseGetPathBoundRect(FixingVector, FixingVector)](M_TFlex_Model_Circuits_LinkBase_GetPathBoundRect.md)) |
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
|  | [GetReferenceToSelectedText](M_TFlex_Model_Circuits_Link_GetReferenceToSelectedText.md) |  |
|  | [GetRegenerationResult](M_TFlex_Model_ModelObject_GetRegenerationResult.md) | Результат пересчета объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRelation](M_TFlex_Model_ModelObject_GetRelation.md) | Измерить отношение двух объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRelationWithUnit](M_TFlex_Model_ModelObject_GetRelationWithUnit.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetSymbols](M_TFlex_Model_Circuits_Link_GetSymbols.md) | Получить все графические обозначения на ЛС |
|  | [GetTextProp](M_TFlex_Model_ModelObject_GetTextProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProperty](M_TFlex_Model_ModelObject_GetTextProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTexts(Boolean, DesignationType)](M_TFlex_Model_Circuits_Link_GetTexts.md) | (Переопределяет [LinkBaseGetTexts(Boolean, DesignationType)](M_TFlex_Model_Circuits_LinkBase_GetTexts.md)) |
|  | [GetTexts(Boolean, FixingVector, DesignationType)](M_TFlex_Model_Circuits_Link_GetTexts_1.md) | (Переопределяет [LinkBaseGetTexts(Boolean, FixingVector, DesignationType)](M_TFlex_Model_Circuits_LinkBase_GetTexts_1.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetWireConnectionInfo(Element, Boolean)](M_TFlex_Model_Circuits_Link_GetWireConnectionInfo_1.md) | (Переопределяет [LinkBaseGetWireConnectionInfo(Element, Boolean)](M_TFlex_Model_Circuits_LinkBase_GetWireConnectionInfo_1.md)) |
|  | [GetWireConnectionInfo(Int32, Boolean)](M_TFlex_Model_Circuits_Link_GetWireConnectionInfo.md) | (Переопределяет [LinkBaseGetWireConnectionInfo(Int32, Boolean)](M_TFlex_Model_Circuits_LinkBase_GetWireConnectionInfo.md)) |
|  | [HasDesignation(DesignationType)](M_TFlex_Model_Circuits_Link_HasDesignation.md) | (Переопределяет [LinkBaseHasDesignation(DesignationType)](M_TFlex_Model_Circuits_LinkBase_HasDesignation.md)) |
|  | [HasDesignation(FixingVector, DesignationType)](M_TFlex_Model_Circuits_Link_HasDesignation_1.md) | (Переопределяет [LinkBaseHasDesignation(FixingVector, DesignationType)](M_TFlex_Model_Circuits_LinkBase_HasDesignation_1.md)) |
|  | [HasDesignations](M_TFlex_Model_Circuits_Link_HasDesignations.md) | (Переопределяет [LinkBaseHasDesignations(DesignationType)](M_TFlex_Model_Circuits_LinkBase_HasDesignations.md)) |
|  | [Insert(FixingVector)](M_TFlex_Model_Circuits_Link_Insert.md) | вставка point1 в линию связи |
|  | [Insert(FixingVector, FixingVector)](M_TFlex_Model_Circuits_Link_Insert_1.md) | вставка point1 и point2 в линию связи |
|  | [InternalRegenerate](M_TFlex_Model_ModelObject_InternalRegenerate.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MarkPath(Graphics, Point, Point)](M_TFlex_Model_Circuits_Link_MarkPath.md) | (Переопределяет [LinkBaseMarkPath(Graphics, Point, Point)](M_TFlex_Model_Circuits_LinkBase_MarkPath.md)) |
|  | [MarkPath(Graphics, FixingVector, FixingVector)](M_TFlex_Model_Circuits_Link_MarkPath_1.md) | (Переопределяет [LinkBaseMarkPath(Graphics, FixingVector, FixingVector)](M_TFlex_Model_Circuits_LinkBase_MarkPath_1.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnBeginEdit](M_TFlex_Model_Circuits_Link_OnBeginEdit.md) | Событие на начало редактирования |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndEdit](M_TFlex_Model_Circuits_Link_OnEndEdit.md) | Событие на завершение редактирования |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RebaseDesignation](M_TFlex_Model_Circuits_Link_RebaseDesignation.md) | (Переопределяет [LinkBaseRebaseDesignation(FixingVector, FixingVector, DesignationType, HashSetIntPtr)](M_TFlex_Model_Circuits_LinkBase_RebaseDesignation.md)) |
|  | [Regenerate](M_TFlex_Model_ModelObject_Regenerate.md) | Пересчитать объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Remove](M_TFlex_Model_Circuits_Link_Remove.md) | (Переопределяет [LinkBaseRemove(FixingVector)](M_TFlex_Model_Circuits_LinkBase_Remove.md)) |
|  | [RemoveChainDesignations](M_TFlex_Model_Circuits_Link_RemoveChainDesignations.md) | (Переопределяет [LinkBaseRemoveChainDesignations](M_TFlex_Model_Circuits_LinkBase_RemoveChainDesignations.md)) |
|  | [RemoveDesignation(DesignationType)](M_TFlex_Model_Circuits_Link_RemoveDesignation.md) | (Переопределяет [LinkBaseRemoveDesignation(DesignationType)](M_TFlex_Model_Circuits_LinkBase_RemoveDesignation.md)) |
|  | [RemoveDesignation(FixingVector, DesignationType)](M_TFlex_Model_Circuits_Link_RemoveDesignation_1.md) | (Переопределяет [LinkBaseRemoveDesignation(FixingVector, DesignationType)](M_TFlex_Model_Circuits_LinkBase_RemoveDesignation_1.md)) |
|  | [RemoveDesignations](M_TFlex_Model_Circuits_Link_RemoveDesignations.md) | (Переопределяет [LinkBaseRemoveDesignations(DesignationType)](M_TFlex_Model_Circuits_LinkBase_RemoveDesignations.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ReplaceDesignation(String, String, String)](M_TFlex_Model_Circuits_Link_ReplaceDesignation.md) | (Переопределяет [LinkBaseReplaceDesignation(String, String, String)](M_TFlex_Model_Circuits_LinkBase_ReplaceDesignation.md)) |
|  | [ReplaceDesignation(String, String, String, String)](M_TFlex_Model_Circuits_Link_ReplaceDesignation_1.md) | (Переопределяет [LinkBaseReplaceDesignation(String, String, String, String)](M_TFlex_Model_Circuits_LinkBase_ReplaceDesignation_1.md)) |
|  | [ReplaceParents](M_TFlex_Model_Circuits_Link_ReplaceParents.md) |  |
|  | [SetDesignation(String, String, DesignationType)](M_TFlex_Model_Circuits_Link_SetDesignation.md) | (Переопределяет [LinkBaseSetDesignation(String, String, DesignationType)](M_TFlex_Model_Circuits_LinkBase_SetDesignation.md)) |
|  | [SetDesignation(String, MultilineText, String)](M_TFlex_Model_Circuits_Link_SetDesignation_2.md) | (Переопределяет [LinkBaseSetDesignation(String, MultilineText, String)](M_TFlex_Model_Circuits_LinkBase_SetDesignation_2.md)) |
|  | [SetDesignation(String, FixingVector, Double, String, DesignationType)](M_TFlex_Model_Circuits_Link_SetDesignation_1.md) | (Переопределяет [LinkBaseSetDesignation(String, FixingVector, Double, String, DesignationType)](M_TFlex_Model_Circuits_LinkBase_SetDesignation_1.md)) |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFontOptions](M_TFlex_Model_Circuits_Link_SetFontOptions.md) | (Переопределяет [LinkBaseSetFontOptions(FontOptions)](M_TFlex_Model_Circuits_LinkBase_SetFontOptions.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_ModelObject_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetTextHorizontalAlignment](M_TFlex_Model_Circuits_Link_SetTextHorizontalAlignment.md) | (Переопределяет [LinkBaseSetTextHorizontalAlignment(TextHorizontalAlignment)](M_TFlex_Model_Circuits_LinkBase_SetTextHorizontalAlignment.md)) |
|  | [SetTextVerticalAlignment](M_TFlex_Model_Circuits_Link_SetTextVerticalAlignment.md) | (Переопределяет [LinkBaseSetTextVerticalAlignment(TextVerticalAlignment)](M_TFlex_Model_Circuits_LinkBase_SetTextVerticalAlignment.md)) |
|  | [ShowDesignations](M_TFlex_Model_Circuits_Link_ShowDesignations.md) | (Переопределяет [LinkBaseShowDesignations(DesignationType, Boolean)](M_TFlex_Model_Circuits_LinkBase_ShowDesignations.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Transform](M_TFlex_Model_Model2D_Object2D_Transform.md) | Применение преобразования.(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [Translate](M_TFlex_Model_Model2D_Object2D_Translate.md) | Сдвиг объекта на данный вектор(Унаследован от [Object2D](T_TFlex_Model_Model2D_Object2D.md)) |
|  | [UpdatePage](M_TFlex_Model_Circuits_Link_UpdatePage.md) |  |
|  | [UpdateScheme](M_TFlex_Model_Circuits_Link_UpdateScheme.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_AddMultilineText.md) | Аггрегировать новый многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineText.md) | Получить аггрегированный многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextBounds](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextBounds.md) | Получить габариты аггрегированного многострочного текста(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextsCount](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextsCount.md) | Количество аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [RemoveMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_RemoveMultilineText.md) | Удалить многострочный текст по индексу(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [UpdateMultilineTextPage](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_UpdateMultilineTextPage.md) | Обновить страницу аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
  
#### Ссылки

[TFlex.Model.Circuits - пространство имён](N_TFlex_Model_Circuits.md)