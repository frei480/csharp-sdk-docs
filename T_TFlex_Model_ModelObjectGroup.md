

Руководство по T-FLEX CAD Open API

# ModelObjectGroup - класс  
    
Класс группы объектов модели, вспомогательного объекта документа T-FLEX.

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelModelObjectGroup

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class ModelObjectGroup
```
```vb
Public NotInheritable Class ModelObjectGroup
```
```cpp
public ref class ModelObjectGroup sealed
```


Тип ModelObjectGroup предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ModelObjectGroup](M_TFlex_Model_ModelObjectGroup__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Attributes](P_TFlex_Model_ModelObjectGroup_Attributes.md) | **Устарело.** |
|  | [Count](P_TFlex_Model_ModelObjectGroup_Count.md) | Количество элементов в группе |
|  | [Document](P_TFlex_Model_ModelObjectGroup_Document.md) | Документ, являющийся родительским для данной группы |
|  | [GroupItems](P_TFlex_Model_ModelObjectGroup_GroupItems.md) | Коллекция элементов, входящих в группу |
|  | [IsOnTopLevel](P_TFlex_Model_ModelObjectGroup_IsOnTopLevel.md) | Возвращает true, если группа не входит в другую группу |
|  | [Name](P_TFlex_Model_ModelObjectGroup_Name.md) | Имя группы |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Add(ModelObject)](M_TFlex_Model_ModelObjectGroup_Add.md) | Добавление объекта в группу |
|  | [Add(ModelObjectGroup)](M_TFlex_Model_ModelObjectGroup_Add_1.md) | Добавление другой группы в данную группу |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindItem(ModelObject)](M_TFlex_Model_ModelObjectGroup_FindItem.md) | Найти элемент группы - объект модели |
|  | [FindItem(ModelObjectGroup)](M_TFlex_Model_ModelObjectGroup_FindItem_1.md) | Найти элемент группы - вложенную группу |
|  | [GetAttributes](M_TFlex_Model_ModelObjectGroup_GetAttributes.md) |  |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Remove(ModelObject)](M_TFlex_Model_ModelObjectGroup_Remove.md) | Удаление объекта из группы |
|  | [Remove(ModelObjectGroup)](M_TFlex_Model_ModelObjectGroup_Remove_1.md) | Удаление вложенной группы объектов из данной группы |
|  | [RemoveAllItems](M_TFlex_Model_ModelObjectGroup_RemoveAllItems.md) | Удаление всех элементов группы |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)