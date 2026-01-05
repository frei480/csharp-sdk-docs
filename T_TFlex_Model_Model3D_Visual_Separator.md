

Руководство по T-FLEX CAD Open API

# Separator - класс  
  
---  
  
Разделитель

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.VisualSceneNode](T_TFlex_Model_Model3D_Visual_SceneNode.md) [TFlex.Model.Model3D.VisualGroup](T_TFlex_Model_Model3D_Visual_Group.md) TFlex.Model.Model3D.VisualSeparator

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Separator : Group
```
```vb
Public Class Separator
	Inherits Group
```
```cpp
public ref class Separator : public Group
```


Тип Separator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Separator](M_TFlex_Model_Model3D_Visual_Separator__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddChild](M_TFlex_Model_Model3D_Visual_Group_AddChild.md) | Узел становится правым потомком группы.(Унаследован от [Group](T_TFlex_Model_Model3D_Visual_Group.md)) |
|  | [CompareTo](M_TFlex_Model_Model3D_Visual_SceneNode_CompareTo.md) | Сравнивает указатели на узлы(Унаследован от [SceneNode](T_TFlex_Model_Model3D_Visual_SceneNode.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_SceneNode_Dispose.md) | (Унаследован от [SceneNode](T_TFlex_Model_Model3D_Visual_SceneNode.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_SceneNode_Dispose_1.md) | (Унаследован от [SceneNode](T_TFlex_Model_Model3D_Visual_SceneNode.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindChild](M_TFlex_Model_Model3D_Visual_Group_FindChild.md) | В случае, если node является потомком группы, возвращает его индекс, иначе возвращает -1.(Унаследован от [Group](T_TFlex_Model_Model3D_Visual_Group.md)) |
|  | [GetChild](M_TFlex_Model_Model3D_Visual_Group_GetChild.md) | Возвращает потомка с заданным индексом, null в случае, если такого не существует.(Унаследован от [Group](T_TFlex_Model_Model3D_Visual_Group.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetNumChildren](M_TFlex_Model_Model3D_Visual_Group_GetNumChildren.md) | Возвращает число потомков группы.(Унаследован от [Group](T_TFlex_Model_Model3D_Visual_Group.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [InsertChild](M_TFlex_Model_Model3D_Visual_Group_InsertChild.md) | Вставляет узел в число потомков.(Унаследован от [Group](T_TFlex_Model_Model3D_Visual_Group.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveChild(Int32)](M_TFlex_Model_Model3D_Visual_Group_RemoveChild.md) | Удаляет потомка с соответствующим индексом. Потомки с большими индексами сдвигаются влево.(Унаследован от [Group](T_TFlex_Model_Model3D_Visual_Group.md)) |
|  | [RemoveChild(SceneNode)](M_TFlex_Model_Model3D_Visual_Group_RemoveChild_1.md) | Удаляет первого найденного потомка.(Унаследован от [Group](T_TFlex_Model_Model3D_Visual_Group.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Объект этого класса изолирует эффекты атрибутов и трансформаций, являющихся его потомками. 

#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)