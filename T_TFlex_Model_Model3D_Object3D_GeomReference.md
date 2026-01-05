

Руководство по T-FLEX CAD Open API

# Object3DGeomReference - класс  
  
---  
  
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObjectReference](T_TFlex_Model_ModelObject_Reference.md) TFlex.Model.Model3DObject3DGeomReference

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class GeomReference : ModelObjectReference
```
```vb
Public Class GeomReference
	Inherits ModelObjectReference
```
```cpp
public ref class GeomReference : public ModelObjectReference
```


Тип Object3DGeomReference предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Object3DGeomReference(ModelAxis)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor.md) | Конструктор ссылки на модельную ось |
|  | [Object3DGeomReference(ModelBodies)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_2.md) | Конструктор ссылки на модельный набор тел |
|  | [Object3DGeomReference(ModelBox)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_4.md) | Конструктор ссылки на модельную границу |
|  | [Object3DGeomReference(ModelCurve)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_6.md) | Конструктор ссылки на модельную кривую |
|  | [Object3DGeomReference(ModelDirection)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_8.md) | Конструктор ссылки на модельное направление |
|  | [Object3DGeomReference(ModelPlane)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_10.md) | Конструктор ссылки на модельную плоскость |
|  | [Object3DGeomReference(ModelPoint3D)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_12.md) | Конструктор ссылки на модельную точку |
|  | [Object3DGeomReference(ModelSurface)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_14.md) | Конструктор ссылки на модельную поверхность |
|  | [Object3DGeomReference(ModelTopol)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_16.md) | Конструктор ссылки на геометрический элемент модельного тела |
|  | [Object3DGeomReference(ModelAxis, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_1.md) | Конструктор ссылки на модельную ось с передаваемым набором флажков |
|  | [Object3DGeomReference(ModelBodies, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_3.md) | Конструктор ссылки на модельный набор тел с передаваемым набором флажков |
|  | [Object3DGeomReference(ModelBox, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_5.md) | Конструктор ссылки на модельную границу с передаваемым набором флажков |
|  | [Object3DGeomReference(ModelCurve, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_7.md) | Конструктор ссылки на модельную кривую с передаваемым набором флажков |
|  | [Object3DGeomReference(ModelDirection, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_9.md) | Конструктор ссылки на модельное направление с передаваемым набором флажков |
|  | [Object3DGeomReference(ModelPlane, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_11.md) | Конструктор ссылки на модельную плоскость с передаваемым набором флажков |
|  | [Object3DGeomReference(ModelPoint3D, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_13.md) | Конструктор ссылки на модельную точку с передаваемым набором флажков |
|  | [Object3DGeomReference(ModelSurface, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_15.md) | Конструктор ссылки на модельную поверхность с передаваемым набором флажков |
|  | [Object3DGeomReference(ModelTopol, UInt32)](M_TFlex_Model_Model3D_Object3D_GeomReference__ctor_17.md) | Конструктор ссылки на геометрический элемент модельного тела с передаваемым набором флажков |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AllowDelete](P_TFlex_Model_ModelObject_Reference_AllowDelete.md) | Не удалять объект при удалении родителя (удалять только ссылку)(Унаследован от [ModelObjectReference](T_TFlex_Model_ModelObject_Reference.md)) |
|  | [DeleteParentObjects](P_TFlex_Model_ModelObject_Reference_DeleteParentObjects.md) | Удалять родительские объекты(Унаследован от [ModelObjectReference](T_TFlex_Model_ModelObject_Reference.md)) |
|  | [Geometry](P_TFlex_Model_Model3D_Object3D_GeomReference_Geometry.md) | Получить родительскую геометрию |
|  | [IgnoreAllowDeteteForOneChild](P_TFlex_Model_ModelObject_Reference_IgnoreAllowDeteteForOneChild.md) | Игнорировать флаг AllowDelete в случае удаления родителя с одним зависимым потомком(Унаследован от [ModelObjectReference](T_TFlex_Model_ModelObject_Reference.md)) |
|  | [IsTopol](P_TFlex_Model_Model3D_Object3D_GeomReference_IsTopol.md) | Получить признак ссылки на геометрический элемент модельного тела |
|  | [Object](P_TFlex_Model_ModelObject_Reference_Object.md) | Родительский объект(Унаследован от [ModelObjectReference](T_TFlex_Model_ModelObject_Reference.md)) |
|  | [States](P_TFlex_Model_ModelObject_Reference_States.md) | Получить набор флагов(Унаследован от [ModelObjectReference](T_TFlex_Model_ModelObject_Reference.md)) |
  
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
|  | [(ModelAxis to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit.md) |  |
|  | [(ModelBodies to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit_1.md) |  |
|  | [(ModelBox to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit_2.md) |  |
|  | [(ModelCurve to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit_3.md) |  |
|  | [(ModelDirection to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit_4.md) |  |
|  | [(ModelPlane to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit_5.md) |  |
|  | [(ModelPoint3D to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit_6.md) |  |
|  | [(ModelSurface to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit_7.md) |  |
|  | [(ModelTopol to Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_GeomReference_op_Implicit_8.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)