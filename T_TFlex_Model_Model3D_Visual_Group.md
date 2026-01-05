

Руководство по T-FLEX CAD Open API

# Group - класс  
  
---  
  
Базовый класс для групп

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.VisualSceneNode](T_TFlex_Model_Model3D_Visual_SceneNode.md) TFlex.Model.Model3D.VisualGroup [TFlex.Model.Model3D.VisualGroupingNode](T_TFlex_Model_Model3D_Visual_GroupingNode.md) [TFlex.Model.Model3D.VisualSeparator](T_TFlex_Model_Model3D_Visual_Separator.md)

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class Group : SceneNode
```
```vb
Public MustInherit Class Group
	Inherits SceneNode
```
```cpp
public ref class Group abstract : public SceneNode
```


Тип Group предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Group](M_TFlex_Model_Model3D_Visual_Group__ctor.md) | Инициализирует новый экземпляр класса Group |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddChild](M_TFlex_Model_Model3D_Visual_Group_AddChild.md) | Узел становится правым потомком группы. |
|  | [CompareTo](M_TFlex_Model_Model3D_Visual_SceneNode_CompareTo.md) | Сравнивает указатели на узлы(Унаследован от [SceneNode](T_TFlex_Model_Model3D_Visual_SceneNode.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_SceneNode_Dispose.md) | (Унаследован от [SceneNode](T_TFlex_Model_Model3D_Visual_SceneNode.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_SceneNode_Dispose_1.md) | (Унаследован от [SceneNode](T_TFlex_Model_Model3D_Visual_SceneNode.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindChild](M_TFlex_Model_Model3D_Visual_Group_FindChild.md) | В случае, если node является потомком группы, возвращает его индекс, иначе возвращает -1. |
|  | [GetChild](M_TFlex_Model_Model3D_Visual_Group_GetChild.md) | Возвращает потомка с заданным индексом, null в случае, если такого не существует. |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetNumChildren](M_TFlex_Model_Model3D_Visual_Group_GetNumChildren.md) | Возвращает число потомков группы. |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InsertChild](M_TFlex_Model_Model3D_Visual_Group_InsertChild.md) | Вставляет узел в число потомков. |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveChild(Int32)](M_TFlex_Model_Model3D_Visual_Group_RemoveChild.md) | Удаляет потомка с соответствующим индексом. Потомки с большими индексами сдвигаются влево. |
|  | [RemoveChild(SceneNode)](M_TFlex_Model_Model3D_Visual_Group_RemoveChild_1.md) | Удаляет первого найденного потомка. |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Класс служит для группировки узлов в дереве сцены. При выводе на экран, поиске и прочих действиях дерево обходится слева направо и сверху вниз. 

#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)