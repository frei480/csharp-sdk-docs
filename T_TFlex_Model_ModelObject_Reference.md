

Руководство по T-FLEX CAD Open API

# ModelObjectReference - класс  
  
---  
  
Класс для передачи ссылки на другой объект модели

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelModelObjectReference [TFlex.Model.Model3DObject3DGeomReference](T_TFlex_Model_Model3D_Object3D_GeomReference.md)

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class Reference
```
```vb
Public Class Reference
```
```cpp
public ref class Reference
```


Тип ModelObjectReference предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ModelObjectReference(ModelObject)](M_TFlex_Model_ModelObject_Reference__ctor_1.md) | Конструктор ссылки по ключу |
|  | [ModelObjectReference(UInt32)](M_TFlex_Model_ModelObject_Reference__ctor.md) | Конструктор пустой ссылки по ключу с передаваемым набором флажков |
|  | [ModelObjectReference(ModelObject, UInt32)](M_TFlex_Model_ModelObject_Reference__ctor_2.md) | Конструктор ссылки по ключу с передаваемым набором флажков |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AllowDelete](P_TFlex_Model_ModelObject_Reference_AllowDelete.md) | Не удалять объект при удалении родителя (удалять только ссылку) |
|  | [DeleteParentObjects](P_TFlex_Model_ModelObject_Reference_DeleteParentObjects.md) | Удалять родительские объекты |
|  | [IgnoreAllowDeteteForOneChild](P_TFlex_Model_ModelObject_Reference_IgnoreAllowDeteteForOneChild.md) | Игнорировать флаг AllowDelete в случае удаления родителя с одним зависимым потомком |
|  | [Object](P_TFlex_Model_ModelObject_Reference_Object.md) | Родительский объект |
|  | [States](P_TFlex_Model_ModelObject_Reference_States.md) | Получить набор флагов |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [(ModelObject to ModelObjectReference)](M_TFlex_Model_ModelObject_Reference_op_Implicit.md) | Оператор установления ссылки на объект |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)