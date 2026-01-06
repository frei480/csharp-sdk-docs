

Руководство по T-FLEX CAD Open API

# BaseTopol - класс  
    
Базовый класс для всех типов (модельных и геометрических) граней, циклов, рёбер и вершин

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) TFlex.Model.Model3D.GeometryBaseTopol [TFlex.Model.Model3D.GeometryModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md) [TFlex.Model.Model3D.GeometryTopol](T_TFlex_Model_Model3D_Geometry_Topol.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BaseTopol : Geometry, 
	IEquatable<BaseTopol>
```
```vb
Public MustInherit Class BaseTopol
	Inherits Geometry
	Implements IEquatable(Of BaseTopol)
```
```cpp
public ref class BaseTopol abstract : public Geometry, 
	IEquatable<BaseTopol^>
```


Тип BaseTopol предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BaseBody](P_TFlex_Model_Model3D_Geometry_BaseTopol_BaseBody.md) | Получить тело, в котором определён элемент |
|  | [Entity](P_TFlex_Model_Model3D_Geometry_BaseTopol_Entity.md) |  |
|  | [Identify](P_TFlex_Model_Model3D_Geometry_BaseTopol_Identify.md) | Уникальный идентификатор элемента |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Transformation](P_TFlex_Model_Model3D_Geometry_BaseTopol_Transformation.md) |  |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md) | (Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(BaseTopol)](M_TFlex_Model_Model3D_Geometry_BaseTopol_Equals.md) |  |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindBoundBox](M_TFlex_Model_Model3D_Geometry_BaseTopol_FindBoundBox.md) | Получить границы элемента |
|  | [FindExtreme](M_TFlex_Model_Model3D_Geometry_BaseTopol_FindExtreme.md) | Найти экстремальную точку на элементе в заданном направлении |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RangePoint](M_TFlex_Model_Model3D_Geometry_BaseTopol_RangePoint.md) | Найти ближайшую точку на элементе к данной точке |
|  | [RangeTopol](M_TFlex_Model_Model3D_Geometry_BaseTopol_RangeTopol.md) | Найти ближайшие расстояние между двумя топологическими элементами |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [m_marker](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_marker.md) |  |
|  | [m_nativeTopolCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTopolCache.md) |  |
|  | [m_nativeTransfBodyCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTransfBodyCache.md) |  |
|  | [m_nativeTransfTopolCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTransfTopolCache.md) |  |
  
Для двух элементов поддерживается функция сравнения

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)