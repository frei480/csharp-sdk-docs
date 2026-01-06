

Руководство по T-FLEX CAD Open API

# Topol - класс  
    
Базовый класс для геометрических граней, циклов, рёбер и вершин

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md) TFlex.Model.Model3D.GeometryTopol [TFlex.Model.Model3D.GeometryEdge](T_TFlex_Model_Model3D_Geometry_Edge.md) [TFlex.Model.Model3D.GeometryFace](T_TFlex_Model_Model3D_Geometry_Face.md) [TFlex.Model.Model3D.GeometryLoop](T_TFlex_Model_Model3D_Geometry_Loop.md) [TFlex.Model.Model3D.GeometryVertex](T_TFlex_Model_Model3D_Geometry_Vertex.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class Topol : BaseTopol
```
```vb
Public MustInherit Class Topol
	Inherits BaseTopol
```
```cpp
public ref class Topol abstract : public BaseTopol
```


Тип Topol предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BaseBody](P_TFlex_Model_Model3D_Geometry_Topol_BaseBody.md) | Получить геометрическое тело, в котором определён элемент(Переопределяет [BaseTopolBaseBody](P_TFlex_Model_Model3D_Geometry_BaseTopol_BaseBody.md)) |
|  | [Body](P_TFlex_Model_Model3D_Geometry_Topol_Body.md) | Получить геометрическое тело, в котором определён элемент |
|  | [Entity](P_TFlex_Model_Model3D_Geometry_BaseTopol_Entity.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Identify](P_TFlex_Model_Model3D_Geometry_BaseTopol_Identify.md) | Уникальный идентификатор элемента(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Transformation](P_TFlex_Model_Model3D_Geometry_BaseTopol_Transformation.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Topol_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом Topol, а при необходимости освобождает также управляемые ресурсы(Переопределяет [GeometryDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md)) |
|  | [Equals(BaseTopol)](M_TFlex_Model_Model3D_Geometry_BaseTopol_Equals.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_Topol_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
|  | [FindBoundBox](M_TFlex_Model_Model3D_Geometry_BaseTopol_FindBoundBox.md) | Получить границы элемента(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [FindExtreme](M_TFlex_Model_Model3D_Geometry_BaseTopol_FindExtreme.md) | Найти экстремальную точку на элементе в заданном направлении(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RangePoint](M_TFlex_Model_Model3D_Geometry_BaseTopol_RangePoint.md) | Найти ближайшую точку на элементе к данной точке(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [RangeTopol](M_TFlex_Model_Model3D_Geometry_BaseTopol_RangeTopol.md) | Найти ближайшие расстояние между двумя топологическими элементами(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(Topol, Topol)](M_TFlex_Model_Model3D_Geometry_Topol_op_Equality.md) |  |
|  | [Inequality(Topol, Topol)](M_TFlex_Model_Model3D_Geometry_Topol_op_Inequality.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [m_marker](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_marker.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [m_nativeTopolCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTopolCache.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [m_nativeTransfBodyCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTransfBodyCache.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [m_nativeTransfTopolCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTransfTopolCache.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
  
Для двух элементов поддерживается функция сравнения

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)