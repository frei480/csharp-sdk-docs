

Руководство по T-FLEX CAD Open API

# RowFilterTerm - класс  
    
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Data.FiltersTermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md) [TFlex.Model.Data.FiltersTerm](T_TFlex_Model_Data_Filters_Term.md) TFlex.Model.Data.ProductStructureRowFilterTerm

**Пространство имён:** [TFlex.Model.Data.ProductStructure](N_TFlex_Model_Data_ProductStructure.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public class RowFilterTerm : Term
```
```vb
Public Class RowFilterTerm
	Inherits Term
```
```cpp
public ref class RowFilterTerm : public Term
```


Тип RowFilterTerm предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [RowFilterTerm](M_TFlex_Model_Data_ProductStructure_RowFilterTerm__ctor.md) | Инициализирует новый экземпляр класса RowFilterTerm |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AsGroup](P_TFlex_Model_Data_Filters_TermGroupItem_AsGroup.md) | Преобразует текущий элемент к типу [TermGroup](T_TFlex_Model_Data_Filters_TermGroup.md) (если он является группой условий)(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [AsTerm](P_TFlex_Model_Data_Filters_Term_AsTerm.md) | Приводит текущий объект к типу [Term](T_TFlex_Model_Data_Filters_Term.md)(Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [IsError](P_TFlex_Model_Data_Filters_TermGroupItem_IsError.md) | Возвращает значение, указывающее, находится ли элемент в ошибочном состоянии(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [IsGroup](P_TFlex_Model_Data_Filters_TermGroupItem_IsGroup.md) | Возвращает значение, указывающее, является ли текущий элемент группой условий(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [IsTerm](P_TFlex_Model_Data_Filters_TermGroupItem_IsTerm.md) | Возвращает значение, указывающее, является ли текущий элемент условием(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [LogicalOperator](P_TFlex_Model_Data_Filters_TermGroupItem_LogicalOperator.md) | Логический оператор, которым текущий элемент соединяется с предыдущим элементом в группе условий (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Operator](P_TFlex_Model_Data_Filters_Term_Operator.md) | Возвращает или задает оператор сравнения(Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [ParameterDescription](P_TFlex_Model_Data_Filters_Term_ParameterDescription.md) | Возвращает описание параметра условия(Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [ParameterID](P_TFlex_Model_Data_ProductStructure_RowFilterTerm_ParameterID.md) |  |
|  | [ParameterName](P_TFlex_Model_Data_Filters_Term_ParameterName.md) | Возвращает имя параметра условия(Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [Value](P_TFlex_Model_Data_Filters_Term_Value.md) | Возвращает или задает значение для сравнения(Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clear](M_TFlex_Model_Data_Filters_Term_Clear.md) | Очищает условие(Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [Clone](M_TFlex_Model_Data_Filters_TermGroupItem_Clone.md) | (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Copy](M_TFlex_Model_Data_ProductStructure_RowFilterTerm_Copy.md) | (Переопределяет [TermGroupItemCopy](M_TFlex_Model_Data_Filters_TermGroupItem_Copy.md)) |
|  | [CopyPropertiesFrom](M_TFlex_Model_Data_Filters_Term_CopyPropertiesFrom.md) | (Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetValue](M_TFlex_Model_Data_Filters_Term_GetValue.md) | (Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [IsEqualTo](M_TFlex_Model_Data_Filters_Term_IsEqualTo.md) | (Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [IsValid](M_TFlex_Model_Data_Filters_TermGroupItem_IsValid.md) | (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Match](M_TFlex_Model_Data_ProductStructure_RowFilterTerm_Match.md) | (Переопределяет [TermGroupItemMatch(Object)](M_TFlex_Model_Data_Filters_TermGroupItem_Match.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ReadXml](M_TFlex_Model_Data_Filters_Term_ReadXml.md) | (Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [SetValue](M_TFlex_Model_Data_Filters_Term_SetValue.md) | (Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [ToString](M_TFlex_Model_Data_Filters_Term_ToString.md) | Возвращает строковое представление условия(Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [WriteXml](M_TFlex_Model_Data_Filters_Term_WriteXml.md) | (Унаследован от [Term](T_TFlex_Model_Data_Filters_Term.md)) |
|  | [XMLDeserialize](M_TFlex_Model_Data_ProductStructure_RowFilterTerm_XMLDeserialize.md) | (Переопределяет [TermGroupItemXMLDeserialize(XmlElement, SerializationContex)](M_TFlex_Model_Data_Filters_TermGroupItem_XMLDeserialize.md)) |
|  | [XMLSerialize](M_TFlex_Model_Data_ProductStructure_RowFilterTerm_XMLSerialize.md) | (Переопределяет [TermGroupItemXMLSerialize(XmlWriter)](M_TFlex_Model_Data_Filters_TermGroupItem_XMLSerialize.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [HeirarchyLevelParamID](F_TFlex_Model_Data_ProductStructure_RowFilterTerm_HeirarchyLevelParamID.md) |  |
  
#### Ссылки

[TFlex.Model.Data.ProductStructure - пространство имён](N_TFlex_Model_Data_ProductStructure.md)