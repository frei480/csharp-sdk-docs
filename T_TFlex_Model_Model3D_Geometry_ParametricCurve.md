

Руководство по T-FLEX CAD Open API

# ParametricCurve - класс  
    
Геометрическая кривая на поверхности с модели

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md) [TFlex.Model.Model3D.GeometryCurve](T_TFlex_Model_Model3D_Geometry_Curve.md) TFlex.Model.Model3D.GeometryParametricCurve

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class ParametricCurve : Curve, 
	BaseParametricCurve
```




Тип ParametricCurve предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ParametricCurve](M_TFlex_Model_Model3D_Geometry_ParametricCurve__ctor.md) | Создание прямой |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Param](P_TFlex_Model_Model3D_Geometry_BaseCurve_Param.md) | Получить информацию о параметризации(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [ParamCurve](P_TFlex_Model_Model3D_Geometry_ParametricCurve_ParamCurve.md) | Получить плоскую кривую, задающую форму кривой в параметрической области поверхности |
|  | [ParasolidCurve](P_TFlex_Model_Model3D_Geometry_BaseCurve_ParasolidCurve.md) | Кривая в формате Parasolid(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Surface](P_TFlex_Model_Model3D_Geometry_ParametricCurve_Surface.md) | Получить поверхность, на которой строится кривая |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ApplyTransform](M_TFlex_Model_Model3D_Geometry_BaseCurve_ApplyTransform.md) | Трансформация кривой(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Binormal](M_TFlex_Model_Model3D_Geometry_BaseCurve_Binormal.md) | Вычислить бинормаль в точке на кривой по параметру(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [ConvertParamByLength](M_TFlex_Model_Model3D_Geometry_BaseCurve_ConvertParamByLength.md) | Конвертировать параметр по длине в параметр кривой(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [ConvertParamByLengthRatio](M_TFlex_Model_Model3D_Geometry_BaseCurve_ConvertParamByLengthRatio.md) | Конвертировать параметр отношения к длине в параметр кривой(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [ConvertToRGK](M_TFlex_Model_Model3D_Geometry_BaseCurve_ConvertToRGK.md) | Конвертировать кривую Parasolid в кривую RGK(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Curvature](M_TFlex_Model_Model3D_Geometry_BaseCurve_Curvature.md) | Вычислить кривизну в точке на кривой по параметру(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Derivative](M_TFlex_Model_Model3D_Geometry_BaseCurve_Derivative.md) | Вычислить производные в точке на кривой по параметру(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseCurve_Dispose.md) | (Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Eval](M_TFlex_Model_Model3D_Geometry_BaseCurve_Eval.md) | Вычислить координаты точки на кривой по параметру(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [EvalPolyline](M_TFlex_Model_Model3D_Geometry_BaseCurve_EvalPolyline.md) | (Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_BaseCurve_Finalize.md) | (Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IntersectCurve](M_TFlex_Model_Model3D_Geometry_BaseCurve_IntersectCurve.md) | Найти пересечение кривой с другой кривой(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Interval](M_TFlex_Model_Model3D_Geometry_BaseCurve_Interval.md) | Вычислить параметрический интервал на кривой, ограниченный двумя точками, лежащими на кривой(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Length](M_TFlex_Model_Model3D_Geometry_BaseCurve_Length.md) | Вычислить длину кривой по параметру(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [MakeReverseCurve](M_TFlex_Model_Model3D_Geometry_BaseCurve_MakeReverseCurve.md) | Трансформация кривой(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Parameterize](M_TFlex_Model_Model3D_Geometry_BaseCurve_Parameterize.md) | Вычислить параметр на кривой, для точки, лежащей на кривой(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [PrincipalNormal](M_TFlex_Model_Model3D_Geometry_BaseCurve_PrincipalNormal.md) | Вычислить главную нормаль в точке на кривой по параметру(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [Tangent](M_TFlex_Model_Model3D_Geometry_BaseCurve_Tangent.md) | Вычислить касательную в точке на кривой по параметру(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Update](M_TFlex_Model_Model3D_Geometry_BaseCurve_Update.md) | Обновить геометрию для каждого конкретного порождённого типа(Унаследован от [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)