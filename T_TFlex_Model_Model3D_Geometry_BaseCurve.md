

Руководство по T-FLEX CAD Open API

# BaseCurve - класс  
  
---  
  
Базовый класс для кривых

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) TFlex.Model.Model3D.GeometryBaseCurve [TFlex.Model.Model3D.GeometryCurve](T_TFlex_Model_Model3D_Geometry_Curve.md) [TFlex.Model.Model3D.GeometryModelCurve](T_TFlex_Model_Model3D_Geometry_ModelCurve.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BaseCurve : Geometry, 
	IDisposable
```
```vb
Public MustInherit Class BaseCurve
	Inherits Geometry
	Implements IDisposable
```
```cpp
public ref class BaseCurve abstract : public Geometry, 
	IDisposable
```


Тип BaseCurve предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Param](P_TFlex_Model_Model3D_Geometry_BaseCurve_Param.md) | Получить информацию о параметризации |
|  | [ParasolidCurve](P_TFlex_Model_Model3D_Geometry_BaseCurve_ParasolidCurve.md) | Кривая в формате Parasolid |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ApplyTransform](M_TFlex_Model_Model3D_Geometry_BaseCurve_ApplyTransform.md) | Трансформация кривой |
|  | [Binormal](M_TFlex_Model_Model3D_Geometry_BaseCurve_Binormal.md) | Вычислить бинормаль в точке на кривой по параметру |
|  | [ConvertParamByLength](M_TFlex_Model_Model3D_Geometry_BaseCurve_ConvertParamByLength.md) | Конвертировать параметр по длине в параметр кривой |
|  | [ConvertParamByLengthRatio](M_TFlex_Model_Model3D_Geometry_BaseCurve_ConvertParamByLengthRatio.md) | Конвертировать параметр отношения к длине в параметр кривой |
|  | [ConvertToRGK](M_TFlex_Model_Model3D_Geometry_BaseCurve_ConvertToRGK.md) | Конвертировать кривую Parasolid в кривую RGK |
|  | [Curvature](M_TFlex_Model_Model3D_Geometry_BaseCurve_Curvature.md) | Вычислить кривизну в точке на кривой по параметру |
|  | [Derivative](M_TFlex_Model_Model3D_Geometry_BaseCurve_Derivative.md) | Вычислить производные в точке на кривой по параметру |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseCurve_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом BaseCurve, а при необходимости освобождает также управляемые ресурсы(Переопределяет [GeometryDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Eval](M_TFlex_Model_Model3D_Geometry_BaseCurve_Eval.md) | Вычислить координаты точки на кривой по параметру |
|  | [EvalPolyline](M_TFlex_Model_Model3D_Geometry_BaseCurve_EvalPolyline.md) |  |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_BaseCurve_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IntersectCurve](M_TFlex_Model_Model3D_Geometry_BaseCurve_IntersectCurve.md) | Найти пересечение кривой с другой кривой |
|  | [Interval](M_TFlex_Model_Model3D_Geometry_BaseCurve_Interval.md) | Вычислить параметрический интервал на кривой, ограниченный двумя точками, лежащими на кривой |
|  | [Length](M_TFlex_Model_Model3D_Geometry_BaseCurve_Length.md) | Вычислить длину кривой по параметру |
|  | [MakeReverseCurve](M_TFlex_Model_Model3D_Geometry_BaseCurve_MakeReverseCurve.md) | Трансформация кривой |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Parameterize](M_TFlex_Model_Model3D_Geometry_BaseCurve_Parameterize.md) | Вычислить параметр на кривой, для точки, лежащей на кривой |
|  | [PrincipalNormal](M_TFlex_Model_Model3D_Geometry_BaseCurve_PrincipalNormal.md) | Вычислить главную нормаль в точке на кривой по параметру |
|  | [Tangent](M_TFlex_Model_Model3D_Geometry_BaseCurve_Tangent.md) | Вычислить касательную в точке на кривой по параметру |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Update](M_TFlex_Model_Model3D_Geometry_BaseCurve_Update.md) | Обновить геометрию для каждого конкретного порождённого типа(Переопределяет Geometry.Update) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)