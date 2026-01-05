

Руководство по T-FLEX CAD Open API

# ModelTopol - класс  
  
---  
  
Базовый класс для модельных граней, циклов, рёбер и вершин

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md) TFlex.Model.Model3D.GeometryModelTopol [TFlex.Model.Model3D.GeometryModelEdge](T_TFlex_Model_Model3D_Geometry_ModelEdge.md) [TFlex.Model.Model3D.GeometryModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md) [TFlex.Model.Model3D.GeometryModelLoop](T_TFlex_Model_Model3D_Geometry_ModelLoop.md) [TFlex.Model.Model3D.GeometryModelVertex](T_TFlex_Model_Model3D_Geometry_ModelVertex.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class ModelTopol : BaseTopol
```
```vb
Public Class ModelTopol
	Inherits BaseTopol
```
```cpp
public ref class ModelTopol : public BaseTopol
```


Тип ModelTopol предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BaseBody](P_TFlex_Model_Model3D_Geometry_ModelTopol_BaseBody.md) | Получить модельное тело, в котором определён элемент(Переопределяет [BaseTopolBaseBody](P_TFlex_Model_Model3D_Geometry_BaseTopol_BaseBody.md)) |
|  | [Body](P_TFlex_Model_Model3D_Geometry_ModelTopol_Body.md) | Получить модельное тело, в котором определён элемент |
|  | [Box](P_TFlex_Model_Model3D_Geometry_ModelTopol_Box.md) | Получить границы элемента |
|  | [Entity](P_TFlex_Model_Model3D_Geometry_BaseTopol_Entity.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [ExistentReference](P_TFlex_Model_Model3D_Geometry_ModelTopol_ExistentReference.md) | Возвращается ссылка, если она существует |
|  | [Identify](P_TFlex_Model_Model3D_Geometry_BaseTopol_Identify.md) | Уникальный идентификатор элемента(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Name](P_TFlex_Model_Model3D_Geometry_ModelTopol_Name.md) | Название элемента |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_ModelTopol_Owner.md) | Получить родительскую операцию |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_ModelTopol_Reference.md) | **Устарело.** Если ссылки не существует, то она создаётся |
|  | [Transformation](P_TFlex_Model_Model3D_Geometry_BaseTopol_Transformation.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CreateReference](M_TFlex_Model_Model3D_Geometry_ModelTopol_CreateReference.md) | Создать ссылку (создается либо топологическая ссылка, либо ссылочный элемент на топологию) |
|  | [CreateReference(Document)](M_TFlex_Model_Model3D_Geometry_ModelTopol_CreateReference_1.md) | Создать ссылку в целевом документ (создается либо топологическая ссылка, либо ссылочный элемент на топологию) |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_ModelTopol_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом ModelTopol, а при необходимости освобождает также управляемые ресурсы(Переопределяет [GeometryDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md)) |
|  | [Equals(BaseTopol)](M_TFlex_Model_Model3D_Geometry_BaseTopol_Equals.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_ModelTopol_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
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
|  | [Equality(ModelTopol, ModelTopol)](M_TFlex_Model_Model3D_Geometry_ModelTopol_op_Equality.md) |  |
|  | [Inequality(ModelTopol, ModelTopol)](M_TFlex_Model_Model3D_Geometry_ModelTopol_op_Inequality.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [m_marker](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_marker.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [m_nativeTopolCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTopolCache.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [m_nativeTransfBodyCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTransfBodyCache.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [m_nativeTransfTopolCache](F_TFlex_Model_Model3D_Geometry_BaseTopol_m_nativeTransfTopolCache.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
  
Для двух элементов поддерживается функция сравнения

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)