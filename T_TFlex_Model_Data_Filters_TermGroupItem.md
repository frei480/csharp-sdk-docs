

Руководство по T-FLEX CAD Open API

# TermGroupItem - класс  
    
Элемент группы условий 

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Data.FiltersTermGroupItem [TFlex.Model.Data.FiltersTerm](T_TFlex_Model_Data_Filters_Term.md) [TFlex.Model.Data.FiltersTermGroup](T_TFlex_Model_Data_Filters_TermGroup.md)

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public abstract class TermGroupItem : ICloneable
```
```vb
Public MustInherit Class TermGroupItem
	Implements ICloneable
```
```cpp
public ref class TermGroupItem abstract : ICloneable
```


Тип TermGroupItem предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [AsGroup](P_TFlex_Model_Data_Filters_TermGroupItem_AsGroup.md) | Преобразует текущий элемент к типу [TermGroup](T_TFlex_Model_Data_Filters_TermGroup.md) (если он является группой условий) |
|  | [AsTerm](P_TFlex_Model_Data_Filters_TermGroupItem_AsTerm.md) | Преобразует текущий элемент к типу [Term](T_TFlex_Model_Data_Filters_Term.md) (если он является условием) |
|  | [IsError](P_TFlex_Model_Data_Filters_TermGroupItem_IsError.md) | Возвращает значение, указывающее, находится ли элемент в ошибочном состоянии |
|  | [IsGroup](P_TFlex_Model_Data_Filters_TermGroupItem_IsGroup.md) | Возвращает значение, указывающее, является ли текущий элемент группой условий |
|  | [IsTerm](P_TFlex_Model_Data_Filters_TermGroupItem_IsTerm.md) | Возвращает значение, указывающее, является ли текущий элемент условием |
|  | [LogicalOperator](P_TFlex_Model_Data_Filters_TermGroupItem_LogicalOperator.md) | Логический оператор, которым текущий элемент соединяется с предыдущим элементом в группе условий |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_Data_Filters_TermGroupItem_Clone.md) |  |
|  | [Copy](M_TFlex_Model_Data_Filters_TermGroupItem_Copy.md) | Создает копию текущего элемента в указанной группе условий |
|  | [CopyPropertiesFrom](M_TFlex_Model_Data_Filters_TermGroupItem_CopyPropertiesFrom.md) |  |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IsEqualTo](M_TFlex_Model_Data_Filters_TermGroupItem_IsEqualTo.md) |  |
|  | [IsValid](M_TFlex_Model_Data_Filters_TermGroupItem_IsValid.md) |  |
|  | [Match](M_TFlex_Model_Data_Filters_TermGroupItem_Match.md) | Возвращает значение, указывающее, соответствует ли указанный объект условиям текущего элемента |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ReadXml](M_TFlex_Model_Data_Filters_TermGroupItem_ReadXml.md) |  |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [WriteXml](M_TFlex_Model_Data_Filters_TermGroupItem_WriteXml.md) |  |
|  | [XMLDeserialize](M_TFlex_Model_Data_Filters_TermGroupItem_XMLDeserialize.md) |  |
|  | [XMLSerialize](M_TFlex_Model_Data_Filters_TermGroupItem_XMLSerialize.md) |  |
  
#### Ссылки

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)