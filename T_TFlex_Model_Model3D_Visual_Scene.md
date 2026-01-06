

Руководство по T-FLEX CAD Open API

# Scene - класс  
    
Класс обеспечивает доступ к трёхмерной сцене документа

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.VisualScene

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class Scene : IEnumerable, 
	IDisposable
```
```vb
Public NotInheritable Class Scene
	Implements IEnumerable, IDisposable
```
```cpp
public ref class Scene sealed : IEnumerable, 
	IDisposable
```


Тип Scene предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Handle](P_TFlex_Model_Model3D_Visual_Scene_Handle.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Add](M_TFlex_Model_Model3D_Visual_Scene_Add.md) | Добавление узла в сцену |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_Scene_Dispose.md) | Освобождает все ресурсы, используемые объектом Scene |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Find](M_TFlex_Model_Model3D_Visual_Scene_Find.md) | Поиск узла, соответствующего данному объекту |
|  | [GetChild](M_TFlex_Model_Model3D_Visual_Scene_GetChild.md) |  |
|  | [GetEnumerator](M_TFlex_Model_Model3D_Visual_Scene_GetEnumerator.md) |  |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetNumChildren](M_TFlex_Model_Model3D_Visual_Scene_GetNumChildren.md) |  |
|  | [GetScene](M_TFlex_Model_Model3D_Visual_Scene_GetScene.md) | Возвращает сцену, принадлежащую данному документу |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Remove](M_TFlex_Model_Model3D_Visual_Scene_Remove.md) | Удаление узла |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Сцена представляет из себя набор узлов, каждый из которых является изображением одного из трёхмерных модельных объектов

#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)