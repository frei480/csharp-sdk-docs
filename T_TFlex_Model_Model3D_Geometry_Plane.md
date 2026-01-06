

Руководство по T-FLEX CAD Open API

# Plane - класс  
    
Геометрическая плоскость

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md) TFlex.Model.Model3D.GeometryPlane

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Plane : BasePlane
```
```vb
Public Class Plane
	Inherits BasePlane
```
```cpp
public ref class Plane : public BasePlane
```


Тип Plane предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Plane(BasePlane)](M_TFlex_Model_Model3D_Geometry_Plane__ctor.md) | Конструктор, копирующий свойства другой плоскости |
|  | [Plane(BasePoint3D, BaseDirection, BaseDirection)](M_TFlex_Model_Model3D_Geometry_Plane__ctor_1.md) | Конструктор для создания геометрической плоскости по точке и двум осям |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Normal](P_TFlex_Model_Model3D_Geometry_Plane_Normal.md) | Нормаль к плоскости |
|  | [Origin](P_TFlex_Model_Model3D_Geometry_Plane_Origin.md) | Нулевая точка плоскости |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [XAxis](P_TFlex_Model_Model3D_Geometry_Plane_XAxis.md) | Направление оси X к плоскости |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_Model3D_Geometry_BasePlane_Clone.md) | (Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md) | (Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equal](M_TFlex_Model_Model3D_Geometry_BasePlane_Equal.md) | Проверка совпадения плоскостей(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [LineIntersection](M_TFlex_Model_Model3D_Geometry_BasePlane_LineIntersection.md) | Получить пересечение плоскости с прямой(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [PlaneIntersection](M_TFlex_Model_Model3D_Geometry_BasePlane_PlaneIntersection.md) | Получить пересечение двух плоскостей(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [PointProjection](M_TFlex_Model_Model3D_Geometry_BasePlane_PointProjection.md) | Получить ортогональную проекцию точки на плоскость(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)