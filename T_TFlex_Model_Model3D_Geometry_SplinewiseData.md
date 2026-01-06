

Руководство по T-FLEX CAD Open API

# SplinewiseData - класс  
    
Класс для задания и определения свойств интерполяционного сплайна по набору точек, через которые проходит сплайн, по параметрам кривой в этих точках и условиям на концах

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometrySplinewiseData

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class SplinewiseData : IDisposable
```
```vb
Public NotInheritable Class SplinewiseData
	Implements IDisposable
```
```cpp
public ref class SplinewiseData sealed : IDisposable
```


Тип SplinewiseData предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [SplinewiseData](M_TFlex_Model_Model3D_Geometry_SplinewiseData__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Begin](P_TFlex_Model_Model3D_Geometry_SplinewiseData_Begin.md) | Условие в начале |
|  | [BeginDerivative](P_TFlex_Model_Model3D_Geometry_SplinewiseData_BeginDerivative.md) | Производная в начале, если условие в начале задаётся производной |
|  | [Degree](P_TFlex_Model_Model3D_Geometry_SplinewiseData_Degree.md) | Получить степень сплайна |
|  | [End](P_TFlex_Model_Model3D_Geometry_SplinewiseData_End.md) | Условие в конце |
|  | [EndDerivative](P_TFlex_Model_Model3D_Geometry_SplinewiseData_EndDerivative.md) | Производная в конце, если условие в конце задаётся производной |
|  | [Knots](P_TFlex_Model_Model3D_Geometry_SplinewiseData_Knots.md) | Параметры для каждой точки задаются в явном виде |
|  | [Points](P_TFlex_Model_Model3D_Geometry_SplinewiseData_Points.md) | Получить интерполяционные точки |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_SplinewiseData_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)