

Руководство по T-FLEX CAD Open API

# Term - класс  
    
Условие фильтра

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Data.FiltersTermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md) TFlex.Model.Data.FiltersTerm [TFlex.Model.Data.ProductStructureObjectTerm](T_TFlex_Model_Data_ProductStructure_ObjectTerm.md) [TFlex.Model.Data.ProductStructureRowFilterTerm](T_TFlex_Model_Data_ProductStructure_RowFilterTerm.md)

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public abstract class Term : TermGroupItem
```
```vb
Public MustInherit Class Term
	Inherits TermGroupItem
```
```cpp
public ref class Term abstract : public TermGroupItem
```


Тип Term предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Term](M_TFlex_Model_Data_Filters_Term__ctor.md) | Инициализирует новый экземпляр класса Term |
|  | [Term(LogicalOperator)](M_TFlex_Model_Data_Filters_Term__ctor_1.md) | Инициализирует новый экземпляр класса Term |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AsGroup](P_TFlex_Model_Data_Filters_TermGroupItem_AsGroup.md) | Преобразует текущий элемент к типу [TermGroup](T_TFlex_Model_Data_Filters_TermGroup.md) (если он является группой условий)(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [AsTerm](P_TFlex_Model_Data_Filters_Term_AsTerm.md) | Приводит текущий объект к типу Term(Переопределяет [TermGroupItemAsTerm](P_TFlex_Model_Data_Filters_TermGroupItem_AsTerm.md)) |
|  | [IsError](P_TFlex_Model_Data_Filters_TermGroupItem_IsError.md) | Возвращает значение, указывающее, находится ли элемент в ошибочном состоянии(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [IsGroup](P_TFlex_Model_Data_Filters_TermGroupItem_IsGroup.md) | Возвращает значение, указывающее, является ли текущий элемент группой условий(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [IsTerm](P_TFlex_Model_Data_Filters_TermGroupItem_IsTerm.md) | Возвращает значение, указывающее, является ли текущий элемент условием(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [LogicalOperator](P_TFlex_Model_Data_Filters_TermGroupItem_LogicalOperator.md) | Логический оператор, которым текущий элемент соединяется с предыдущим элементом в группе условий (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Operator](P_TFlex_Model_Data_Filters_Term_Operator.md) | Возвращает или задает оператор сравнения |
|  | [ParameterDescription](P_TFlex_Model_Data_Filters_Term_ParameterDescription.md) | Возвращает описание параметра условия |
|  | [ParameterName](P_TFlex_Model_Data_Filters_Term_ParameterName.md) | Возвращает имя параметра условия |
|  | [Value](P_TFlex_Model_Data_Filters_Term_Value.md) | Возвращает или задает значение для сравнения |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clear](M_TFlex_Model_Data_Filters_Term_Clear.md) | Очищает условие |
|  | [Clone](M_TFlex_Model_Data_Filters_TermGroupItem_Clone.md) | (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Copy](M_TFlex_Model_Data_Filters_TermGroupItem_Copy.md) | Создает копию текущего элемента в указанной группе условий(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [CopyPropertiesFrom](M_TFlex_Model_Data_Filters_Term_CopyPropertiesFrom.md) | (Переопределяет [TermGroupItemCopyPropertiesFrom(TermGroupItem)](M_TFlex_Model_Data_Filters_TermGroupItem_CopyPropertiesFrom.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetValue](M_TFlex_Model_Data_Filters_Term_GetValue.md) |  |
|  | [IsEqualTo](M_TFlex_Model_Data_Filters_Term_IsEqualTo.md) | (Переопределяет [TermGroupItemIsEqualTo(TermGroupItem)](M_TFlex_Model_Data_Filters_TermGroupItem_IsEqualTo.md)) |
|  | [IsValid](M_TFlex_Model_Data_Filters_TermGroupItem_IsValid.md) | (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [Match](M_TFlex_Model_Data_Filters_TermGroupItem_Match.md) | Возвращает значение, указывающее, соответствует ли указанный объект условиям текущего элемента(Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ReadXml](M_TFlex_Model_Data_Filters_Term_ReadXml.md) | (Переопределяет [TermGroupItemReadXml(XmlElement)](M_TFlex_Model_Data_Filters_TermGroupItem_ReadXml.md)) |
|  | [SetValue](M_TFlex_Model_Data_Filters_Term_SetValue.md) |  |
|  | [ToString](M_TFlex_Model_Data_Filters_Term_ToString.md) | Возвращает строковое представление условия(Переопределяет [ObjectToString](https://learn.microsoft.com/dotnet/api/system.object.tostring)) |
|  | [WriteXml](M_TFlex_Model_Data_Filters_Term_WriteXml.md) | (Переопределяет [TermGroupItemWriteXml(XmlWriter)](M_TFlex_Model_Data_Filters_TermGroupItem_WriteXml.md)) |
|  | [XMLDeserialize](M_TFlex_Model_Data_Filters_TermGroupItem_XMLDeserialize.md) | (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
|  | [XMLSerialize](M_TFlex_Model_Data_Filters_TermGroupItem_XMLSerialize.md) | (Унаследован от [TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)) |
  
#### Ссылки

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)