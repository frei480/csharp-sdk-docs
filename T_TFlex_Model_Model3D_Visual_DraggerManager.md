

Руководство по T-FLEX CAD Open API

# DraggerManager - класс  
  
---  
  
**Примечание: Данный API устарел.**

Диспетчер манипуляторов

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.VisualDraggerManager

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")]
public sealed class DraggerManager : IDisposable
```
```vb
<ObsoleteAttribute("This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")>
Public NotInheritable Class DraggerManager
	Implements IDisposable
```
```cpp
[ObsoleteAttribute(L"This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")]
public ref class DraggerManager sealed : IDisposable
```


Тип DraggerManager предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Owner](P_TFlex_Model_Model3D_Visual_DraggerManager_Owner.md) | Возвращает документ, с которым связан диспетчер |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDragger](M_TFlex_Model_Model3D_Visual_DraggerManager_AddDragger.md) | Регистрирует манипулятор |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_DraggerManager_Dispose.md) | Освобождает все ресурсы, используемые объектом DraggerManager |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetDragger](M_TFlex_Model_Model3D_Visual_DraggerManager_GetDragger.md) | Возвращает манипулятор с заданным идентификатором |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetManager](M_TFlex_Model_Model3D_Visual_DraggerManager_GetManager.md) | Возвращает диспетчер манипуляторов, связанный с заданным документом |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveAllDraggers](M_TFlex_Model_Model3D_Visual_DraggerManager_RemoveAllDraggers.md) | Удаляет все манипуляторы |
|  | [RemoveDragger(Dragger)](M_TFlex_Model_Model3D_Visual_DraggerManager_RemoveDragger_1.md) | Удаляет манипулятор |
|  | [RemoveDragger(Int32)](M_TFlex_Model_Model3D_Visual_DraggerManager_RemoveDragger.md) | Удаляет манипулятор с заданным идентификатором |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Для того, чтобы манипулятор изображался в 3D окне и мог выбираться, нужно зарегистрировать его в диспетчере соответствующего документа. 

#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)

[DecorationManager](T_TFlex_Model_Model3D_Visual_DecorationManager.md)

[Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)

[DecorationManager](T_TFlex_Model_Model3D_Visual_DecorationManager.md)

[Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)