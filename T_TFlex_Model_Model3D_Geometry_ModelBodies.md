

Руководство по T-FLEX CAD Open API

# ModelBodies - класс  
    
Множество тел с объекта модели

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBodies](T_TFlex_Model_Model3D_Geometry_Bodies.md) TFlex.Model.Model3D.GeometryModelBodies [TFlex.Model.Model3D.GeometryModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md) [TFlex.Model.Model3D.GeometryModelSolid](T_TFlex_Model_Model3D_Geometry_ModelSolid.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class ModelBodies : Bodies, 
	IEnumerator, IEnumerable, IDisposable
```
```vb
Public MustInherit Class ModelBodies
	Inherits Bodies
	Implements IEnumerator, IEnumerable, IDisposable
```
```cpp
public ref class ModelBodies abstract : public Bodies, 
	IEnumerator, IEnumerable, IDisposable
```


Тип ModelBodies предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Current](P_TFlex_Model_Model3D_Geometry_ModelBodies_Current.md) | Получить текущий элемент |
|  | [Item](P_TFlex_Model_Model3D_Geometry_ModelBodies_Item.md) |  |
|  | [Length](P_TFlex_Model_Model3D_Geometry_ModelBodies_Length.md) | Количество тел |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_ModelBodies_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом ModelBodies, а при необходимости освобождает также управляемые ресурсы(Переопределяет [GeometryDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Find](M_TFlex_Model_Model3D_Geometry_ModelBodies_Find.md) |  |
|  | [FindByChain](M_TFlex_Model_Model3D_Geometry_ModelBodies_FindByChain.md) |  |
|  | [GetEnumerator](M_TFlex_Model_Model3D_Geometry_ModelBodies_GetEnumerator.md) | Получить перечислитель |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveNext](M_TFlex_Model_Model3D_Geometry_ModelBodies_MoveNext.md) | Перейти к следующему элементу |
|  | [Reset](M_TFlex_Model_Model3D_Geometry_ModelBodies_Reset.md) | Сбросить перечислитель |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)