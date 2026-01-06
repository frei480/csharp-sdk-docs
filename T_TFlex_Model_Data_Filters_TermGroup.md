

Руководство по T-FLEX CAD Open API

# TermGroup - класс  
    
Группа условий фильтра 

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Data.FiltersTermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md) TFlex.Model.Data.FiltersTermGroup

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public sealed class TermGroup : TermGroupItem, 
	IList<TermGroupItem>, ICollection<TermGroupItem>, IEnumerable<TermGroupItem>, 
	IEnumerable
```




Тип TermGroup предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [TermGroup](M_TFlex_Model_Data_Filters_TermGroup__ctor.md) | Создает новую группу условий |
|  | [TermGroup(LogicalOperator)](M_TFlex_Model_Data_Filters_TermGroup__ctor_1.md) | Инициализирует новый экземпляр класса TermGroup |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AsGroup](P_TFlex_Model_Data_Filters_TermGroup_AsGroup.md) | Приводит текущий объект к типу TermGroup(Переопределяет [TermGroupItemAsGroup](P_TFlex_Model_Data_Filters_TermGroupItem_AsGroup.md)) |
|  | [AsTerm](P_TFlex_Model_Data_Filters_TermGroupItem_AsTerm.md) | Преобразует текущий элемент к типу [Term](T_TFlex_Model_Data_Filters_Term.md) (если он является условием)(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Count](P_TFlex_Model_Data_Filters_TermGroup_Count.md) | Возвращает количество элементов в группе условий |
|  | [IsError](P_TFlex_Model_Data_Filters_TermGroupItem_IsError.md) | Возвращает значение, указывающее, находится ли элемент в ошибочном состоянии(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [IsGroup](P_TFlex_Model_Data_Filters_TermGroupItem_IsGroup.md) | Возвращает значение, указывающее, является ли текущий элемент группой условий(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [IsReadOnly](P_TFlex_Model_Data_Filters_TermGroup_IsReadOnly.md) | Возвращает значение, указывающее, является ли группа условий доступной только для чтения |
|  | [IsTerm](P_TFlex_Model_Data_Filters_TermGroupItem_IsTerm.md) | Возвращает значение, указывающее, является ли текущий элемент условием(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Item](P_TFlex_Model_Data_Filters_TermGroup_Item.md) | Возвращает элемент, находящийся в группе условий по указанному индексу |
|  | [LogicalOperator](P_TFlex_Model_Data_Filters_TermGroupItem_LogicalOperator.md) | Логический оператор, которым текущий элемент соединяется с предыдущим элементом в группе условий (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Add](M_TFlex_Model_Data_Filters_TermGroup_Add.md) | Добавляет указанный элемент в текущую группу условий |
|  | [AddGroup](M_TFlex_Model_Data_Filters_TermGroup_AddGroup.md) | Добавляет дочернюю группу условий в текущую группу |
|  | [Clear](M_TFlex_Model_Data_Filters_TermGroup_Clear.md) | Очищает текущую группу условий |
|  | [Clone](M_TFlex_Model_Data_Filters_TermGroupItem_Clone.md) | (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Contains](M_TFlex_Model_Data_Filters_TermGroup_Contains.md) | Возвращает значение, указывающее, содержится ли заданный элемент в группе условий |
|  | [Copy](M_TFlex_Model_Data_Filters_TermGroup_Copy.md) | Копирует текущую группу условий (Переопределяет [TermGroupItemCopy](M_TFlex_Model_Data_Filters_TermGroupItem_Copy.md)) |
|  | [CopyPropertiesFrom](M_TFlex_Model_Data_Filters_TermGroup_CopyPropertiesFrom.md) | (Переопределяет [TermGroupItemCopyPropertiesFrom(TermGroupItem)](M_TFlex_Model_Data_Filters_TermGroupItem_CopyPropertiesFrom.md)) |
|  | [CopyTo](M_TFlex_Model_Data_Filters_TermGroup_CopyTo.md) | Копирует элементы группы условий в заданный массив элементов, начиная с указанного индекса |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_Model_Data_Filters_TermGroup_GetEnumerator.md) | Возвращает перечислитель элементов в группе условий |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetText](M_TFlex_Model_Data_Filters_TermGroup_GetText.md) | Возвращает текстовое представление группы условий |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IndexOf](M_TFlex_Model_Data_Filters_TermGroup_IndexOf.md) | Возвращает индекс указанного элемента в текущей группе условий |
|  | [Insert](M_TFlex_Model_Data_Filters_TermGroup_Insert.md) | Добавляет в текущую группу условий указанный элемент по заданному индексу |
|  | [IsEqualTo](M_TFlex_Model_Data_Filters_TermGroup_IsEqualTo.md) | (Переопределяет [TermGroupItemIsEqualTo(TermGroupItem)](M_TFlex_Model_Data_Filters_TermGroupItem_IsEqualTo.md)) |
|  | [Match](M_TFlex_Model_Data_Filters_TermGroup_Match.md) | Возвращает значение, указывающее, соответствует ли указанный объект условиям группы(Переопределяет [TermGroupItemMatch(Object)](M_TFlex_Model_Data_Filters_TermGroupItem_Match.md)) |
|  | [Remove](M_TFlex_Model_Data_Filters_TermGroup_Remove.md) | Удаляет указанный элемент из текущей группы условий |
|  | [RemoveAt](M_TFlex_Model_Data_Filters_TermGroup_RemoveAt.md) | Удаляет из текущей группы условий элемент с указанным индексом |
|  | [RemoveEmptyGroups](M_TFlex_Model_Data_Filters_TermGroup_RemoveEmptyGroups.md) | Удаляет из текущей группы элементы, которые являются пустыми группами |
|  | [RemoveErrorItems](M_TFlex_Model_Data_Filters_TermGroup_RemoveErrorItems.md) | Удаляет из текущей группы элементы, которые находятся в ошибочном состоянии |
|  | [ToString](M_TFlex_Model_Data_Filters_TermGroup_ToString.md) | Возвращает строковое представление группы условий(Переопределяет [ObjectToString](https://learn.microsoft.com/dotnet/api/system.object.tostring)) |
|  | [XMLDeserialize](M_TFlex_Model_Data_Filters_TermGroup_XMLDeserialize.md) | (Переопределяет [TermGroupItemXMLDeserialize(XmlElement, SerializationContex)](M_TFlex_Model_Data_Filters_TermGroupItem_XMLDeserialize.md)) |
|  | [XMLSerialize](M_TFlex_Model_Data_Filters_TermGroup_XMLSerialize.md) | (Переопределяет [TermGroupItemXMLSerialize(XmlWriter)](M_TFlex_Model_Data_Filters_TermGroupItem_XMLSerialize.md)) |
  
#### Ссылки

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)