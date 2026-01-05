

Руководство по T-FLEX CAD Open API

# OverrideCollectionT \- класс  
  
---  
  
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Data.ProductStructureOverrideCollectionT [TFlex.Model.Data.ProductStructureBoolOverrideCollection](T_TFlex_Model_Data_ProductStructure_BoolOverrideCollection.md)

**Пространство имён:** [TFlex.Model.Data.ProductStructure](N_TFlex_Model_Data_ProductStructure.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public abstract class OverrideCollection<T> : ICloneable
where T : struct, new(), IComparable<T>

```
```vb
Public MustInherit Class OverrideCollection(Of T As {Structure, New, IComparable(Of T)})
	Implements ICloneable
```
```cpp
generic<typename T>
where T : value class, gcnew(), IComparable<T>
public ref class OverrideCollection abstract : ICloneable
```


#### Параметры типа

T
    

Тип OverrideCollectionT предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [OverrideCollectionT](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1__ctor.md) | Инициализирует новый экземпляр класса OverrideCollectionT |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [IsEmpty](P_TFlex_Model_Data_ProductStructure_OverrideCollection_1_IsEmpty.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ClearAll](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_ClearAll.md) |  |
|  | [ClearOverride](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_ClearOverride.md) |  |
|  | [Clone](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_Clone.md) |  |
|  | [CopyCollection](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_CopyCollection.md) |  |
|  | [Equals](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_Equals.md) | (Переопределяет [ObjectEquals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\))) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_GetHashCode.md) | (Переопределяет [ObjectGetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetValue](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_GetValue.md) |  |
|  | [IsOverriding](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_IsOverriding.md) |  |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ReadValue](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_ReadValue.md) |  |
|  | [SetOverride](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_SetOverride.md) |  |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [WriteValue](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_WriteValue.md) |  |
|  | [XMLDeserialize](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_XMLDeserialize.md) |  |
|  | [XMLSerialize](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_XMLSerialize.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(OverrideCollectionT, OverrideCollectionT)](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_op_Equality.md) |  |
|  | [Inequality(OverrideCollectionT, OverrideCollectionT)](M_TFlex_Model_Data_ProductStructure_OverrideCollection_1_op_Inequality.md) |  |
  
#### Ссылки

[TFlex.Model.Data.ProductStructure - пространство имён](N_TFlex_Model_Data_ProductStructure.md)