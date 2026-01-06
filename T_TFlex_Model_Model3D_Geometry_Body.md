

Руководство по T-FLEX CAD Open API

# Body - класс  
    
Класс хранения геометрических тел

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryBaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md) TFlex.Model.Model3D.GeometryBody

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Body : BaseBody, IDisposable
```
```vb
Public Class Body
	Inherits BaseBody
	Implements IDisposable
```
```cpp
public ref class Body : public BaseBody, 
	IDisposable
```


Тип Body предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Body(BaseBody)](M_TFlex_Model_Model3D_Geometry_Body__ctor_1.md) | Конструктор для создания тела как копии другого тела |
|  | [Body(BaseFace)](M_TFlex_Model_Model3D_Geometry_Body__ctor_2.md) | Конструктор для создания листового тела на основе грани |
|  | [Body(Int32)](M_TFlex_Model_Model3D_Geometry_Body__ctor.md) | Инициализирует новый экземпляр класса Body |
|  | [Body(BasePoint3D, BasePoint3D, BasePoint3D)](M_TFlex_Model_Model3D_Geometry_Body__ctor_3.md) | Конструктор для создания листового прямоугольника(параллелограмма) |
|  | [Body(BasePoint3D, BasePoint3D, BasePoint3D, BasePoint3D)](M_TFlex_Model_Model3D_Geometry_Body__ctor_4.md) | Конструктор для создания параллелепипеда |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [BodyHandle](P_TFlex_Model_Model3D_Geometry_BaseBody_BodyHandle.md) | (Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Edges](P_TFlex_Model_Model3D_Geometry_Body_Edges.md) | Множество рёбер(Переопределяет [BaseBodyEdges](P_TFlex_Model_Model3D_Geometry_BaseBody_Edges.md)) |
|  | [Existence](P_TFlex_Model_Model3D_Geometry_Body_Existence.md) | Признак существования тела |
|  | [Faces](P_TFlex_Model_Model3D_Geometry_Body_Faces.md) | Множество граней(Переопределяет [BaseBodyFaces](P_TFlex_Model_Model3D_Geometry_BaseBody_Faces.md)) |
|  | [IsClosedIfWire](P_TFlex_Model_Model3D_Geometry_BaseBody_IsClosedIfWire.md) | Если тело является контуром, то можно проверить его замкнутость(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [LengthIfWire](P_TFlex_Model_Model3D_Geometry_BaseBody_LengthIfWire.md) | Если тело является контуром, то можно получить его длину(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Loops](P_TFlex_Model_Model3D_Geometry_Body_Loops.md) | Множество циклов(Переопределяет [BaseBodyLoops](P_TFlex_Model_Model3D_Geometry_BaseBody_Loops.md)) |
|  | [NormalIfPlanarSheet](P_TFlex_Model_Model3D_Geometry_BaseBody_NormalIfPlanarSheet.md) | Для плоского листового тела возвращается нормаль к лицевой стороне тела(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [PlaneIfWire](P_TFlex_Model_Model3D_Geometry_BaseBody_PlaneIfWire.md) | Если тело является контуром, то можно проверить его планарность и получить плоскость, в которой он лежит(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Transformation](P_TFlex_Model_Model3D_Geometry_BaseBody_Transformation.md) | (Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Type](P_TFlex_Model_Model3D_Geometry_BaseBody_Type.md) | (Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Vertices](P_TFlex_Model_Model3D_Geometry_Body_Vertices.md) | Множество вершин(Переопределяет [BaseBodyVertices](P_TFlex_Model_Model3D_Geometry_BaseBody_Vertices.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ApplyTransform](M_TFlex_Model_Model3D_Geometry_BaseBody_ApplyTransform.md) | Трансформация геометрии тела(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Check](M_TFlex_Model_Model3D_Geometry_BaseBody_Check.md) | Проверить тело Parasolid(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Clash](M_TFlex_Model_Model3D_Geometry_BaseBody_Clash.md) | Функция определяет столкновение тел(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [ClashBody](M_TFlex_Model_Model3D_Geometry_BaseBody_ClashBody.md) | **Устарело.** Функция определяет перекрытие тел(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [ContainsPoint](M_TFlex_Model_Model3D_Geometry_BaseBody_ContainsPoint.md) | Функция определяет положение точки относительно тела(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [ConvertToRGK(Document, IntPtr)](M_TFlex_Model_Model3D_Geometry_BaseBody_ConvertToRGK.md) | Конвертировать тело Parasolid в тело RGK(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [ConvertToRGK(Document, IntPtr, BaseBodyConvertToRGKOptions)](M_TFlex_Model_Model3D_Geometry_BaseBody_ConvertToRGK_1.md) | Конвертировать тело Parasolid в тело RGK(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Detach](M_TFlex_Model_Model3D_Geometry_BaseBody_Detach.md) | (Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BaseBody_Dispose.md) | (Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Body_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом Body, а при необходимости освобождает также управляемые ресурсы(Переопределяет [BaseBodyDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseBody_Dispose_1.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Facet](M_TFlex_Model_Model3D_Geometry_BaseBody_Facet.md) | Функция создаёт плоскогранную сетку(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_BaseBody_Finalize.md) | (Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [FindBoundBox](M_TFlex_Model_Model3D_Geometry_BaseBody_FindBoundBox.md) | Получить границы тела(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [FindExtreme](M_TFlex_Model_Model3D_Geometry_BaseBody_FindExtreme.md) | Найти экстремальную точку на теле в заданном направлении(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IntersectWire](M_TFlex_Model_Model3D_Geometry_BaseBody_IntersectWire.md) | (Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [NormalizeIfPlanarClosedWire](M_TFlex_Model_Model3D_Geometry_Body_NormalizeIfPlanarClosedWire.md) | Если тело является плоским замкнутым контуром, то обход по нему можно ориентировать против часовой стрелки согласно нормали к этой плоскости |
|  | [RangePoint(BasePoint3D)](M_TFlex_Model_Model3D_Geometry_BaseBody_RangePoint.md) | Найти точку на теле ближайшую к данной точке(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [RangePoint(BasePoint3D, Point3D, UV)](M_TFlex_Model_Model3D_Geometry_BaseBody_RangePoint_1.md) | Найти точку на теле ближайшую к данной точке(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [RangeTopol(BaseBody)](M_TFlex_Model_Model3D_Geometry_BaseBody_RangeTopol.md) | Найти ближайшие расстояние между двумя телами(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [RangeTopol(BaseTopol)](M_TFlex_Model_Model3D_Geometry_BaseBody_RangeTopol_1.md) | Найти ближайшее расстояние между телом и топологическим элементом(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [ReverseIfWire](M_TFlex_Model_Model3D_Geometry_Body_ReverseIfWire.md) | Если тело является контуром, то можно изменить ориентацию контура |
|  | [SetApprox](M_TFlex_Model_Model3D_Geometry_BaseBody_SetApprox.md) | Функция формирует набор вспомогательных данных, ускоряющих выполнение функции [ContainsPoint(BasePoint3D)](M_TFlex_Model_Model3D_Geometry_BaseBody_ContainsPoint.md), если выполняется несколько вызовов этой функции(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [UnsetApprox](M_TFlex_Model_Model3D_Geometry_BaseBody_UnsetApprox.md) | Если ранее была вызвана функция [SetApprox](M_TFlex_Model_Model3D_Geometry_BaseBody_SetApprox.md), то по завершении работы нужно вызвать функцию удаления вспомогательных данных(Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
|  | [WireEval](M_TFlex_Model_Model3D_Geometry_BaseBody_WireEval.md) | (Унаследован от [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)