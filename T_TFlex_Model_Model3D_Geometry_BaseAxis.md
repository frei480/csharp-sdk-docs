

Руководство по T-FLEX CAD Open API

# BaseAxis - класс  
  
---  
  
Базовый класс для оси

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) TFlex.Model.Model3D.GeometryBaseAxis [TFlex.Model.Model3D.GeometryAxis](T_TFlex_Model_Model3D_Geometry_Axis.md) [TFlex.Model.Model3D.GeometryModelAxis](T_TFlex_Model_Model3D_Geometry_ModelAxis.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BaseAxis : Geometry
```
```vb
Public MustInherit Class BaseAxis
	Inherits Geometry
```
```cpp
public ref class BaseAxis abstract : public Geometry
```


Тип BaseAxis предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Direction](P_TFlex_Model_Model3D_Geometry_BaseAxis_Direction.md) | Вектор направления оси |
|  | [Origin](P_TFlex_Model_Model3D_Geometry_BaseAxis_Origin.md) | Точка, через которую проходит ось |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md) | (Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [LineIntersection](M_TFlex_Model_Model3D_Geometry_BaseAxis_LineIntersection.md) | Получить пересечение двух прямых |
|  | [LineNearPoints](M_TFlex_Model_Model3D_Geometry_BaseAxis_LineNearPoints.md) | Получить точку на прямой, ближайшую к другой прямой |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [PointProjection](M_TFlex_Model_Model3D_Geometry_BaseAxis_PointProjection.md) | Получить ортогональную проекцию точки на прямую |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Update](M_TFlex_Model_Model3D_Geometry_BaseAxis_Update.md) | Обновить геометрию для каждого конкретного порождённого типа(Переопределяет Geometry.Update) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(BaseAxis, BaseAxis)](M_TFlex_Model_Model3D_Geometry_BaseAxis_op_Equality.md) |  |
|  | [Inequality(BaseAxis, BaseAxis)](M_TFlex_Model_Model3D_Geometry_BaseAxis_op_Inequality.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)