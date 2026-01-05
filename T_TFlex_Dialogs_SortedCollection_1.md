

Руководство по T-FLEX CAD Open API

# SortedCollectionT \- класс  
  
---  
  
Упорядоченная коллекция элементов

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.DialogsSortedCollectionT [TFlex.DialogsSelectedRowCollection](T_TFlex_Dialogs_SelectedRowCollection.md)

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class SortedCollection<T> : ICollection<T>, 
	IReadOnlyList<T>

```
```vb
Public MustInherit Class SortedCollection(Of T)
	Implements ICollection(Of T), IReadOnlyList(Of T)
```
```cpp
generic<typename T>
public ref class SortedCollection abstract : ICollection<T>, 
	IReadOnlyList<T>
```


#### Параметры типа

T
    

Тип SortedCollectionT предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Count](P_TFlex_Dialogs_SortedCollection_1_Count.md) | Получить количество элементов в коллекции |
|  | [IsReadOnly](P_TFlex_Dialogs_SortedCollection_1_IsReadOnly.md) | Коллекция только для чтения |
|  | [Item](P_TFlex_Dialogs_SortedCollection_1_Item.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Add](M_TFlex_Dialogs_SortedCollection_1_Add.md) | Добавить элемент в конец коллекции |
|  | [Add_ICollectionT](M_TFlex_Dialogs_SortedCollection_1_Add_ICollectionT.md) |  |
|  | [Clear](M_TFlex_Dialogs_SortedCollection_1_Clear.md) | Удалить все элементы из коллекции |
|  | [Contains](M_TFlex_Dialogs_SortedCollection_1_Contains.md) | Возвращает true, если коллекция содержит элемент |
|  | [CopyTo](M_TFlex_Dialogs_SortedCollection_1_CopyTo.md) | Копировать коллекцию в массив |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_Dialogs_SortedCollection_1_GetEnumerator.md) | Получить объект для перечисления коллекции |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IEnumerable_GetEnumerator](M_TFlex_Dialogs_SortedCollection_1_IEnumerable_GetEnumerator.md) |  |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Remove](M_TFlex_Dialogs_SortedCollection_1_Remove.md) | Удалить элемент из коллекции |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)