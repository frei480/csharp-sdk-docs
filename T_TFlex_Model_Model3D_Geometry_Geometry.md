

Руководство по T-FLEX CAD Open API

# Geometry - класс  
  
---  
  
Базовый класс для геометрических данных объектов 3D модели

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometryGeometry Подробнее

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class Geometry : IObjectGeometry, 
	IDisposable
```
```vb
Public MustInherit Class Geometry
	Implements IObjectGeometry, IDisposable
```
```cpp
public ref class Geometry abstract : IObjectGeometry, 
	IDisposable
```


Тип Geometry предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом Geometry, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometryGeometry [TFlex.Model.Model3D.GeometryBaseAxis](T_TFlex_Model_Model3D_Geometry_BaseAxis.md) [TFlex.Model.Model3D.GeometryBaseBox](T_TFlex_Model_Model3D_Geometry_BaseBox.md) [TFlex.Model.Model3D.GeometryBaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md) [TFlex.Model.Model3D.GeometryBaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md) [TFlex.Model.Model3D.GeometryBasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md) [TFlex.Model.Model3D.GeometryBasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md) [TFlex.Model.Model3D.GeometryBaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md) [TFlex.Model.Model3D.GeometryBaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md) [TFlex.Model.Model3D.GeometryBodies](T_TFlex_Model_Model3D_Geometry_Bodies.md)