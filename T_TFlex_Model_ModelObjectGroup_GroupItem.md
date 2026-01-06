

Руководство по T-FLEX CAD Open API

# ModelObjectGroupGroupItem - класс  
    
Класс элемента группы объектов.

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelModelObjectGroupGroupItem

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class GroupItem : IDisposable
```
```vb
Public NotInheritable Class GroupItem
	Implements IDisposable
```
```cpp
public ref class GroupItem sealed : IDisposable
```


Тип ModelObjectGroupGroupItem предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Group](P_TFlex_Model_ModelObjectGroup_GroupItem_Group.md) | Вложенная группа, представляемая данным элементом. Если элемент является объектом модели, возвращает null |
|  | [IsGroup](P_TFlex_Model_ModelObjectGroup_GroupItem_IsGroup.md) | Возвращает true, если элемент является вложенной группой |
|  | [IsObject](P_TFlex_Model_ModelObjectGroup_GroupItem_IsObject.md) | Возвращает true, если элемент является объектом |
|  | [Object](P_TFlex_Model_ModelObjectGroup_GroupItem_Object.md) | Объект модели, представляемый данным элементом. Если элемент является вложенной группой, возвращает null |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_ModelObjectGroup_GroupItem_Dispose.md) | Освобождает все ресурсы, используемые объектом ModelObjectGroupGroupItem |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)