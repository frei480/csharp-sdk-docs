

Руководство по T-FLEX CAD Open API

# SceneNode - класс  
  
---  
  
Базовый класс для элементов, входящих в состав изображения модельного объекта. Из объектов данного класса строится дерево трехмерной сцены.

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.VisualSceneNode [TFlex.Model.Model3D.VisualExternalNode](T_TFlex_Model_Model3D_Visual_ExternalNode.md) [TFlex.Model.Model3D.VisualGroup](T_TFlex_Model_Model3D_Visual_Group.md) [TFlex.Model.Model3D.VisualRenderSwitch](T_TFlex_Model_Model3D_Visual_RenderSwitch.md)

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class SceneNode : IDisposable, 
	IComparable
```
```vb
Public MustInherit Class SceneNode
	Implements IDisposable, IComparable
```
```cpp
public ref class SceneNode abstract : IDisposable, 
	IComparable
```


Тип SceneNode предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [SceneNode](M_TFlex_Model_Model3D_Visual_SceneNode__ctor.md) | Инициализирует новый экземпляр класса SceneNode |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CompareTo](M_TFlex_Model_Model3D_Visual_SceneNode_CompareTo.md) | Сравнивает указатели на узлы |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_SceneNode_Dispose.md) | Освобождает все ресурсы, используемые объектом SceneNode |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_SceneNode_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом SceneNode, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(SceneNode, SceneNode)](M_TFlex_Model_Model3D_Visual_SceneNode_op_Equality.md) | Сравнивает указатели на узлы |
|  | [Inequality(SceneNode, SceneNode)](M_TFlex_Model_Model3D_Visual_SceneNode_op_Inequality.md) | Сравнивает указатели на узлы |
  
#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)