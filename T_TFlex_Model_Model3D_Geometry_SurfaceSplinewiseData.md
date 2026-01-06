

Руководство по T-FLEX CAD Open API

# SurfaceSplinewiseData - класс  
    
Класс для задания и определения свойств интерполяционной сплайновой поверхности по набору точек, через которые проходит сплайновая поверхность, по параметрам поверхности в этих точках и условиям на концах

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometrySurfaceSplinewiseData

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class SurfaceSplinewiseData : IDisposable
```




Тип SurfaceSplinewiseData предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [SurfaceSplinewiseData](M_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [LowerUBoundary](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_LowerUBoundary.md) | Получить условия по границе, соответствующей изопараметрической кривой по нижнему значению U |
|  | [LowerULowerV](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_LowerULowerV.md) | Получить закон кручения в вершине, заданной нижним значением U и нижним значением V |
|  | [LowerUUpperV](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_LowerUUpperV.md) | Получить закон кручения в вершине, заданной нижним значением U и верхним значением V |
|  | [LowerVBoundary](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_LowerVBoundary.md) | Получить условия по границе, соответствующей изопараметрической кривой по нижнему значению V |
|  | [Points](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_Points.md) | Получить интерполяционные точки |
|  | [UDegree](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_UDegree.md) | Степень сплайна по U |
|  | [UKnots](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_UKnots.md) | Получить параметры узлов по U |
|  | [UpperUBoundary](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_UpperUBoundary.md) | Получить условия по границе, соответствующей изопараметрической кривой по верхнему значению U |
|  | [UpperULowerV](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_UpperULowerV.md) | Получить закон кручения в вершине, заданной верхним значением U и нижним значением V |
|  | [UpperUUpperV](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_UpperUUpperV.md) | Получить закона кручения в вершине, заданной верхним значением U и верхним значением V |
|  | [UpperVBoundary](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_UpperVBoundary.md) | Получить условия по границе, соответствующей изопараметрической кривой по верхнему значению V |
|  | [VDegree](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_VDegree.md) | Степень сплайна по V |
|  | [VKnots](P_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_VKnots.md) | Получить параметры узлов по V |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)