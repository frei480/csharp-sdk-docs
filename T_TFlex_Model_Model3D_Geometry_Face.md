

Руководство по T-FLEX CAD Open API

# Face - класс  
  
---  
  
Геометрическая грань

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md) [TFlex.Model.Model3D.GeometryTopol](T_TFlex_Model_Model3D_Geometry_Topol.md) TFlex.Model.Model3D.GeometryFace

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class Face : Topol, BaseFace
```
```vb
Public NotInheritable Class Face
	Inherits Topol
	Implements BaseFace
```
```cpp
public ref class Face sealed : public Topol, 
	BaseFace
```


Тип Face предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BaseBody](P_TFlex_Model_Model3D_Geometry_Topol_BaseBody.md) | Получить геометрическое тело, в котором определён элемент(Унаследован от [Topol](T_TFlex_Model_Model3D_Geometry_Topol.md)) |
|  | [Body](P_TFlex_Model_Model3D_Geometry_Topol_Body.md) | Получить геометрическое тело, в котором определён элемент(Унаследован от [Topol](T_TFlex_Model_Model3D_Geometry_Topol.md)) |
|  | [Edges](P_TFlex_Model_Model3D_Geometry_Face_Edges.md) | Множество рёбер |
|  | [Entity](P_TFlex_Model_Model3D_Geometry_BaseTopol_Entity.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Identify](P_TFlex_Model_Model3D_Geometry_BaseTopol_Identify.md) | Уникальный идентификатор элемента(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Loops](P_TFlex_Model_Model3D_Geometry_Face_Loops.md) | Множество циклов |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Sense](P_TFlex_Model_Model3D_Geometry_Face_Sense.md) | Получить признак совпадения ориентации поверхности и грани |
|  | [Surface](P_TFlex_Model_Model3D_Geometry_Face_Surface.md) | Получить поверхность, на которой лежит грань |
|  | [Transformation](P_TFlex_Model_Model3D_Geometry_BaseTopol_Transformation.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [UVBox](P_TFlex_Model_Model3D_Geometry_Face_UVBox.md) | Получить UVbox грани |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Vertices](P_TFlex_Model_Model3D_Geometry_Face_Vertices.md) | Множество вершин |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(BaseTopol)](M_TFlex_Model_Model3D_Geometry_BaseTopol_Equals.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindAxis](M_TFlex_Model_Model3D_Geometry_Face_FindAxis.md) |  |
|  | [FindBoundBox](M_TFlex_Model_Model3D_Geometry_BaseTopol_FindBoundBox.md) | Получить границы элемента(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [FindExtreme](M_TFlex_Model_Model3D_Geometry_BaseTopol_FindExtreme.md) | Найти экстремальную точку на элементе в заданном направлении(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IntersectCurve](M_TFlex_Model_Model3D_Geometry_Face_IntersectCurve.md) | Ищет пересечения между указываемым участком кривой и гранью. |
|  | [IntersectFace](M_TFlex_Model_Model3D_Geometry_Face_IntersectFace.md) | Найти пересечение грани с другой гранью |
|  | [IntersectSurface](M_TFlex_Model_Model3D_Geometry_Face_IntersectSurface.md) | Найти пересечение грани с другой поверхностью |
|  | [OutputSurfTrimmed](M_TFlex_Model_Model3D_Geometry_Face_OutputSurfTrimmed.md) | Возвращает обрезанную поверхность |
|  | [RangePoint](M_TFlex_Model_Model3D_Geometry_BaseTopol_RangePoint.md) | Найти ближайшую точку на элементе к данной точке(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [RangeTopol](M_TFlex_Model_Model3D_Geometry_BaseTopol_RangeTopol.md) | Найти ближайшие расстояние между двумя топологическими элементами(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)