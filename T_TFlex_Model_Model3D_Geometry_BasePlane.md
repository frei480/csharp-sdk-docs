

Руководство по T-FLEX CAD Open API

# BasePlane - класс  
    
Базовый класс для плоскостей

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) TFlex.Model.Model3D.GeometryBasePlane [TFlex.Model.Model3D.GeometryModelPlane](T_TFlex_Model_Model3D_Geometry_ModelPlane.md) [TFlex.Model.Model3D.GeometryPlane](T_TFlex_Model_Model3D_Geometry_Plane.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BasePlane : Geometry
```
```vb
Public MustInherit Class BasePlane
	Inherits Geometry
```
```cpp
public ref class BasePlane abstract : public Geometry
```


Тип BasePlane предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Normal](P_TFlex_Model_Model3D_Geometry_BasePlane_Normal.md) | Получить нормаль к плоскости |
|  | [Origin](P_TFlex_Model_Model3D_Geometry_BasePlane_Origin.md) | Получить нулевую точку плоскости |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [XAxis](P_TFlex_Model_Model3D_Geometry_BasePlane_XAxis.md) | Получить направление оси X к плоскости |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_Model3D_Geometry_BasePlane_Clone.md) |  |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md) | (Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equal](M_TFlex_Model_Model3D_Geometry_BasePlane_Equal.md) | Проверка совпадения плоскостей |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [LineIntersection](M_TFlex_Model_Model3D_Geometry_BasePlane_LineIntersection.md) | Получить пересечение плоскости с прямой |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [PlaneIntersection](M_TFlex_Model_Model3D_Geometry_BasePlane_PlaneIntersection.md) | Получить пересечение двух плоскостей |
|  | [PointProjection](M_TFlex_Model_Model3D_Geometry_BasePlane_PointProjection.md) | Получить ортогональную проекцию точки на плоскость |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(BasePlane, BasePlane)](M_TFlex_Model_Model3D_Geometry_BasePlane_op_Equality.md) |  |
|  | [Inequality(BasePlane, BasePlane)](M_TFlex_Model_Model3D_Geometry_BasePlane_op_Inequality.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)