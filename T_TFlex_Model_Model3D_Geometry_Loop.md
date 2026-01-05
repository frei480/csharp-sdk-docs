

Руководство по T-FLEX CAD Open API

# Loop - класс  
  
---  
  
Геометрический цикл

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md) [TFlex.Model.Model3D.GeometryTopol](T_TFlex_Model_Model3D_Geometry_Topol.md) TFlex.Model.Model3D.GeometryLoop

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class Loop : Topol, BaseLoop
```
```vb
Public NotInheritable Class Loop
	Inherits Topol
	Implements BaseLoop
```
```cpp
public ref class Loop sealed : public Topol, 
	BaseLoop
```


Тип Loop предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BaseBody](P_TFlex_Model_Model3D_Geometry_Topol_BaseBody.md) | Получить геометрическое тело, в котором определён элемент(Унаследован от [Topol](T_TFlex_Model_Model3D_Geometry_Topol.md)) |
|  | [Body](P_TFlex_Model_Model3D_Geometry_Topol_Body.md) | Получить геометрическое тело, в котором определён элемент(Унаследован от [Topol](T_TFlex_Model_Model3D_Geometry_Topol.md)) |
|  | [Edges](P_TFlex_Model_Model3D_Geometry_Loop_Edges.md) | Множество рёбер, образующих цикл |
|  | [Entity](P_TFlex_Model_Model3D_Geometry_BaseTopol_Entity.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Faces](P_TFlex_Model_Model3D_Geometry_Loop_Faces.md) | Грань, которой принадлежит цикл |
|  | [Identify](P_TFlex_Model_Model3D_Geometry_BaseTopol_Identify.md) | Уникальный идентификатор элемента(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [LoopType](P_TFlex_Model_Model3D_Geometry_Loop_LoopType.md) | Тип цикла |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Transformation](P_TFlex_Model_Model3D_Geometry_BaseTopol_Transformation.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Vertices](P_TFlex_Model_Model3D_Geometry_Loop_Vertices.md) | Множество вершин, принадлежащих циклу |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(BaseTopol)](M_TFlex_Model_Model3D_Geometry_BaseTopol_Equals.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindBoundBox](M_TFlex_Model_Model3D_Geometry_BaseTopol_FindBoundBox.md) | Получить границы элемента(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [FindExtreme](M_TFlex_Model_Model3D_Geometry_BaseTopol_FindExtreme.md) | Найти экстремальную точку на элементе в заданном направлении(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RangePoint](M_TFlex_Model_Model3D_Geometry_BaseTopol_RangePoint.md) | Найти ближайшую точку на элементе к данной точке(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [RangeTopol](M_TFlex_Model_Model3D_Geometry_BaseTopol_RangeTopol.md) | Найти ближайшие расстояние между двумя топологическими элементами(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)