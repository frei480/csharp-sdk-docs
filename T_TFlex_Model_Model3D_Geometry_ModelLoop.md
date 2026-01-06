

Руководство по T-FLEX CAD Open API

# ModelLoop - класс  
    
Модельный цикл

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md) [TFlex.Model.Model3D.GeometryModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md) TFlex.Model.Model3D.GeometryModelLoop

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class ModelLoop : ModelTopol, 
	BaseLoop
```
```vb
Public NotInheritable Class ModelLoop
	Inherits ModelTopol
	Implements BaseLoop
```
```cpp
public ref class ModelLoop sealed : public ModelTopol, 
	BaseLoop
```


Тип ModelLoop предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BaseBody](P_TFlex_Model_Model3D_Geometry_ModelTopol_BaseBody.md) | Получить модельное тело, в котором определён элемент(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
|  | [Body](P_TFlex_Model_Model3D_Geometry_ModelTopol_Body.md) | Получить модельное тело, в котором определён элемент(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
|  | [Box](P_TFlex_Model_Model3D_Geometry_ModelTopol_Box.md) | Получить границы элемента(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
|  | [Edges](P_TFlex_Model_Model3D_Geometry_ModelLoop_Edges.md) | Множество рёбер, образующих цикл |
|  | [Entity](P_TFlex_Model_Model3D_Geometry_BaseTopol_Entity.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [ExistentReference](P_TFlex_Model_Model3D_Geometry_ModelTopol_ExistentReference.md) | Возвращается ссылка, если она существует(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
|  | [Faces](P_TFlex_Model_Model3D_Geometry_ModelLoop_Faces.md) | Грань, которой принадлежит цикл |
|  | [Geometry](P_TFlex_Model_Model3D_Geometry_ModelLoop_Geometry.md) | Получить геометрические данные цикла |
|  | [Identify](P_TFlex_Model_Model3D_Geometry_BaseTopol_Identify.md) | Уникальный идентификатор элемента(Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [LoopType](P_TFlex_Model_Model3D_Geometry_ModelLoop_LoopType.md) | Тип цикла |
|  | [Name](P_TFlex_Model_Model3D_Geometry_ModelTopol_Name.md) | Название элемента(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_ModelTopol_Owner.md) | Получить родительскую операцию(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_ModelTopol_Reference.md) | **Устарело.** Если ссылки не существует, то она создаётся(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
|  | [Transformation](P_TFlex_Model_Model3D_Geometry_BaseTopol_Transformation.md) | (Унаследован от [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Vertices](P_TFlex_Model_Model3D_Geometry_ModelLoop_Vertices.md) | Множество вершин, принадлежащих циклу |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CreateReference](M_TFlex_Model_Model3D_Geometry_ModelTopol_CreateReference.md) | Создать ссылку (создается либо топологическая ссылка, либо ссылочный элемент на топологию)(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
|  | [CreateReference(Document)](M_TFlex_Model_Model3D_Geometry_ModelTopol_CreateReference_1.md) | Создать ссылку в целевом документ (создается либо топологическая ссылка, либо ссылочный элемент на топологию)(Унаследован от [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)) |
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