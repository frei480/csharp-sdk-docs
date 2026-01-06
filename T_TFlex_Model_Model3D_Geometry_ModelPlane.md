

Руководство по T-FLEX CAD Open API

# ModelPlane - класс  
    
Плоскость модели

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md) TFlex.Model.Model3D.GeometryModelPlane

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class ModelPlane : BasePlane
```
```vb
Public NotInheritable Class ModelPlane
	Inherits BasePlane
```
```cpp
public ref class ModelPlane sealed : public BasePlane
```


Тип ModelPlane предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Normal](P_TFlex_Model_Model3D_Geometry_BasePlane_Normal.md) | Получить нормаль к плоскости(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [Origin](P_TFlex_Model_Model3D_Geometry_BasePlane_Origin.md) | Получить нулевую точку плоскости(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [XAxis](P_TFlex_Model_Model3D_Geometry_BasePlane_XAxis.md) | Получить направление оси X к плоскости(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_Model3D_Geometry_BasePlane_Clone.md) | (Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equal](M_TFlex_Model_Model3D_Geometry_BasePlane_Equal.md) | Проверка совпадения плоскостей(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [LineIntersection](M_TFlex_Model_Model3D_Geometry_BasePlane_LineIntersection.md) | Получить пересечение плоскости с прямой(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [PlaneIntersection](M_TFlex_Model_Model3D_Geometry_BasePlane_PlaneIntersection.md) | Получить пересечение двух плоскостей(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [PointProjection](M_TFlex_Model_Model3D_Geometry_BasePlane_PointProjection.md) | Получить ортогональную проекцию точки на плоскость(Унаследован от [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)