

Руководство по T-FLEX CAD Open API

# Point3D - класс  
    
Геометрическая точка

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md) TFlex.Model.Model3D.GeometryPoint3D

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Point3D : BasePoint3D
```




Тип Point3D предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Point3D(BasePoint3D)](M_TFlex_Model_Model3D_Geometry_Point3D__ctor_1.md) | Конструктор, копирующий координаты другой точки |
|  | [Point3D(Double, Double, Double)](M_TFlex_Model_Model3D_Geometry_Point3D__ctor.md) | Конструктор для создания геометрической точки по координатам |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Item](P_TFlex_Model_Model3D_Geometry_Point3D_Item.md) |  |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [X](P_TFlex_Model_Model3D_Geometry_Point3D_X.md) | X - координата точки |
|  | [Y](P_TFlex_Model_Model3D_Geometry_Point3D_Y.md) | Y - координата точки |
|  | [Z](P_TFlex_Model_Model3D_Geometry_Point3D_Z.md) | Z - координата точки |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_Model3D_Geometry_BasePoint3D_Clone.md) | (Унаследован от [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md) | (Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Distance](M_TFlex_Model_Model3D_Geometry_BasePoint3D_Distance.md) | Получить расстояние до заданной точки(Унаследован от [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Rotate](M_TFlex_Model_Model3D_Geometry_Point3D_Rotate.md) |  |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Addition(Point3D, Direction)](M_TFlex_Model_Model3D_Geometry_Point3D_op_Addition.md) |  |
|  | [Multiply(Point3D, Double)](M_TFlex_Model_Model3D_Geometry_Point3D_op_Multiply.md) |  |
|  | [Subtraction(Point3D, Direction)](M_TFlex_Model_Model3D_Geometry_Point3D_op_Subtraction.md) |  |
  
Задаётся своими координатами

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)