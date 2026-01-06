

Руководство по T-FLEX CAD Open API

# BaseBody - класс  
    
Базовый класс хранения тел

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometryBaseBody [TFlex.Model.Model3D.GeometryBody](T_TFlex_Model_Model3D_Geometry_Body.md) [TFlex.Model.Model3D.GeometryModelBody](T_TFlex_Model_Model3D_Geometry_ModelBody.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BaseBody : IDisposable
```




Тип BaseBody предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BodyHandle](P_TFlex_Model_Model3D_Geometry_BaseBody_BodyHandle.md) |  |
|  | [Edges](P_TFlex_Model_Model3D_Geometry_BaseBody_Edges.md) | Множество рёбер |
|  | [Faces](P_TFlex_Model_Model3D_Geometry_BaseBody_Faces.md) | Множество граней |
|  | [IsClosedIfWire](P_TFlex_Model_Model3D_Geometry_BaseBody_IsClosedIfWire.md) | Если тело является контуром, то можно проверить его замкнутость |
|  | [LengthIfWire](P_TFlex_Model_Model3D_Geometry_BaseBody_LengthIfWire.md) | Если тело является контуром, то можно получить его длину |
|  | [Loops](P_TFlex_Model_Model3D_Geometry_BaseBody_Loops.md) | Множество циклов |
|  | [NormalIfPlanarSheet](P_TFlex_Model_Model3D_Geometry_BaseBody_NormalIfPlanarSheet.md) | Для плоского листового тела возвращается нормаль к лицевой стороне тела |
|  | [PlaneIfWire](P_TFlex_Model_Model3D_Geometry_BaseBody_PlaneIfWire.md) | Если тело является контуром, то можно проверить его планарность и получить плоскость, в которой он лежит |
|  | [Transformation](P_TFlex_Model_Model3D_Geometry_BaseBody_Transformation.md) |  |
|  | [Type](P_TFlex_Model_Model3D_Geometry_BaseBody_Type.md) |  |
|  | [Vertices](P_TFlex_Model_Model3D_Geometry_BaseBody_Vertices.md) | Множество вершин |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ApplyTransform](M_TFlex_Model_Model3D_Geometry_BaseBody_ApplyTransform.md) | Трансформация геометрии тела |
|  | [Check](M_TFlex_Model_Model3D_Geometry_BaseBody_Check.md) | Проверить тело Parasolid |
|  | [CheckAllBodies](M_TFlex_Model_Model3D_Geometry_BaseBody_CheckAllBodies.md) | Проверить все тела Parasolid |
|  | [CheckBodies](M_TFlex_Model_Model3D_Geometry_BaseBody_CheckBodies.md) |  |
|  | [Clash](M_TFlex_Model_Model3D_Geometry_BaseBody_Clash.md) | Функция определяет столкновение тел |
|  | [ClashBody](M_TFlex_Model_Model3D_Geometry_BaseBody_ClashBody.md) | **Устарело.** Функция определяет перекрытие тел |
|  | [ContainsPoint](M_TFlex_Model_Model3D_Geometry_BaseBody_ContainsPoint.md) | Функция определяет положение точки относительно тела |
|  | [ConvertToRGK(Document, IntPtr)](M_TFlex_Model_Model3D_Geometry_BaseBody_ConvertToRGK.md) | Конвертировать тело Parasolid в тело RGK |
|  | [ConvertToRGK(Document, IntPtr, BaseBodyConvertToRGKOptions)](M_TFlex_Model_Model3D_Geometry_BaseBody_ConvertToRGK_1.md) | Конвертировать тело Parasolid в тело RGK |
|  | [Detach](M_TFlex_Model_Model3D_Geometry_BaseBody_Detach.md) |  |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BaseBody_Dispose.md) | Освобождает все ресурсы, используемые объектом BaseBody |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseBody_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом BaseBody, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Facet](M_TFlex_Model_Model3D_Geometry_BaseBody_Facet.md) | Функция создаёт плоскогранную сетку |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_BaseBody_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
|  | [FindBoundBox](M_TFlex_Model_Model3D_Geometry_BaseBody_FindBoundBox.md) | Получить границы тела |
|  | [FindExtreme](M_TFlex_Model_Model3D_Geometry_BaseBody_FindExtreme.md) | Найти экстремальную точку на теле в заданном направлении |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IntersectWire](M_TFlex_Model_Model3D_Geometry_BaseBody_IntersectWire.md) |  |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RangePoint(BasePoint3D)](M_TFlex_Model_Model3D_Geometry_BaseBody_RangePoint.md) | Найти точку на теле ближайшую к данной точке |
|  | [RangePoint(BasePoint3D, Point3D, UV)](M_TFlex_Model_Model3D_Geometry_BaseBody_RangePoint_1.md) | Найти точку на теле ближайшую к данной точке |
|  | [RangeTopol(BaseBody)](M_TFlex_Model_Model3D_Geometry_BaseBody_RangeTopol.md) | Найти ближайшие расстояние между двумя телами |
|  | [RangeTopol(BaseTopol)](M_TFlex_Model_Model3D_Geometry_BaseBody_RangeTopol_1.md) | Найти ближайшее расстояние между телом и топологическим элементом |
|  | [SetApprox](M_TFlex_Model_Model3D_Geometry_BaseBody_SetApprox.md) | Функция формирует набор вспомогательных данных, ускоряющих выполнение функции [ContainsPoint(BasePoint3D)](M_TFlex_Model_Model3D_Geometry_BaseBody_ContainsPoint.md), если выполняется несколько вызовов этой функции |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [UnsetApprox](M_TFlex_Model_Model3D_Geometry_BaseBody_UnsetApprox.md) | Если ранее была вызвана функция [SetApprox](M_TFlex_Model_Model3D_Geometry_BaseBody_SetApprox.md), то по завершении работы нужно вызвать функцию удаления вспомогательных данных |
|  | [WireEval](M_TFlex_Model_Model3D_Geometry_BaseBody_WireEval.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)