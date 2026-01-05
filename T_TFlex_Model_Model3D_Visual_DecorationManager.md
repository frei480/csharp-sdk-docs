

Руководство по T-FLEX CAD Open API

# DecorationManager - класс  
  
---  
  
Диспетчер декораций

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.VisualDecorationManager

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class DecorationManager : IDisposable
```
```vb
Public NotInheritable Class DecorationManager
	Implements IDisposable
```
```cpp
public ref class DecorationManager sealed : IDisposable
```


Тип DecorationManager предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Owner](P_TFlex_Model_Model3D_Visual_DecorationManager_Owner.md) | Документ, соответствующий диспетчеру |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDecoration](M_TFlex_Model_Model3D_Visual_DecorationManager_AddDecoration.md) | Регистрация декорации |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_DecorationManager_Dispose.md) | Освобождает все ресурсы, используемые объектом DecorationManager |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetDecoration](M_TFlex_Model_Model3D_Visual_DecorationManager_GetDecoration.md) | Поиск декорации |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetManager](M_TFlex_Model_Model3D_Visual_DecorationManager_GetManager.md) | Получение диспетчера для соответствующего документа |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveAllDecorations](M_TFlex_Model_Model3D_Visual_DecorationManager_RemoveAllDecorations.md) | Удаление всех декораций |
|  | [RemoveDecoration](M_TFlex_Model_Model3D_Visual_DecorationManager_RemoveDecoration.md) | Удаление декорации |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Для того, чтобы декорация стала видимой, ее нужно добавить в диспетчер соответствующего документа

#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)

[Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)

[DraggerManager](T_TFlex_Model_Model3D_Visual_DraggerManager.md)