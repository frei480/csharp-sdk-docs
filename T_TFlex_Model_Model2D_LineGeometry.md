

Руководство по T-FLEX CAD Open API

# LineGeometry - класс  
    
Класс 2D геометрии - отрезок или прямая

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model2DObjectGeometry](T_TFlex_Model_Model2D_ObjectGeometry.md) TFlex.Model.Model2DLineGeometry

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class LineGeometry : ObjectGeometry
```
```vb
Public Class LineGeometry
	Inherits ObjectGeometry
```
```cpp
public ref class LineGeometry : public ObjectGeometry
```


Тип LineGeometry предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [LineGeometry](M_TFlex_Model_Model2D_LineGeometry__ctor.md) | Конструктор, инициализирующий параметры геометрии |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Type](P_TFlex_Model_Model2D_LineGeometry_Type.md) | Тип геометрии(Переопределяет [ObjectGeometryType](P_TFlex_Model_Model2D_ObjectGeometry_Type.md)) |
|  | [X1](P_TFlex_Model_Model2D_LineGeometry_X1.md) | X-координата первой точки прямой или начала отрезка |
|  | [X2](P_TFlex_Model_Model2D_LineGeometry_X2.md) | X-координата второй точки прямой или конца отрезка |
|  | [Y1](P_TFlex_Model_Model2D_LineGeometry_Y1.md) | Y-координата первой точки прямой или начала отрезка |
|  | [Y2](P_TFlex_Model_Model2D_LineGeometry_Y2.md) | Y-координата второй точки прямой или конца отрезка |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model2D_ObjectGeometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [ObjectGeometry](T_TFlex_Model_Model2D_ObjectGeometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model2D_ObjectGeometry_Dispose_1.md) | (Унаследован от [ObjectGeometry](T_TFlex_Model_Model2D_ObjectGeometry.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetDistance](M_TFlex_Model_Model2D_ObjectGeometry_GetDistance.md) | Минимальное расстояние до точки(Унаследован от [ObjectGeometry](T_TFlex_Model_Model2D_ObjectGeometry.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)