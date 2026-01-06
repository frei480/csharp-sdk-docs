

Руководство по T-FLEX CAD Open API

# BaseSurface - класс  
    
Базовый класс для поверхностей

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) TFlex.Model.Model3D.GeometryBaseSurface [TFlex.Model.Model3D.GeometryModelSurface](T_TFlex_Model_Model3D_Geometry_ModelSurface.md) [TFlex.Model.Model3D.GeometrySurface](T_TFlex_Model_Model3D_Geometry_Surface.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BaseSurface : Geometry, 
	IDisposable
```




Тип BaseSurface предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [ParasolidSurface](P_TFlex_Model_Model3D_Geometry_BaseSurface_ParasolidSurface.md) |  |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [UParam](P_TFlex_Model_Model3D_Geometry_BaseSurface_UParam.md) | Получить информацию о параметризации по U |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [VParam](P_TFlex_Model_Model3D_Geometry_BaseSurface_VParam.md) | Получить информацию о параметризации по V |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ApplyTransform](M_TFlex_Model_Model3D_Geometry_BaseSurface_ApplyTransform.md) | Трансформация поверхности |
|  | [Derivative](M_TFlex_Model_Model3D_Geometry_BaseSurface_Derivative.md) | Вычислить производные в точке на поверхности по параметрам |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseSurface_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом BaseSurface, а при необходимости освобождает также управляемые ресурсы(Переопределяет [GeometryDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Eval](M_TFlex_Model_Model3D_Geometry_BaseSurface_Eval.md) | Вычислить координаты точки на поверхности по параметрам |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_BaseSurface_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IntersectCurve](M_TFlex_Model_Model3D_Geometry_BaseSurface_IntersectCurve.md) | Найти пересечение поверхности с кривой |
|  | [IntersectSurface](M_TFlex_Model_Model3D_Geometry_BaseSurface_IntersectSurface.md) | Найти пересечение поверхности с другой поверхностью |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Normal](M_TFlex_Model_Model3D_Geometry_BaseSurface_Normal.md) | Вычислить нормаль к поверхности в точке по параметрам |
|  | [Parameterize](M_TFlex_Model_Model3D_Geometry_BaseSurface_Parameterize.md) | Вычислить параметр на поверхности, для точки, лежащей на поверхности |
|  | [Parameterize2](M_TFlex_Model_Model3D_Geometry_BaseSurface_Parameterize2.md) | Вычислить параметры на поверхности, для точки, лежащей около нее |
|  | [PrincipalCurvature1](M_TFlex_Model_Model3D_Geometry_BaseSurface_PrincipalCurvature1.md) | Вычислить первую главную кривизну в точек на поверхности по параметрам |
|  | [PrincipalCurvature2](M_TFlex_Model_Model3D_Geometry_BaseSurface_PrincipalCurvature2.md) | Вычислить вторую главную кривизну в точках на поверхности по параметрам |
|  | [PrincipalDirection1](M_TFlex_Model_Model3D_Geometry_BaseSurface_PrincipalDirection1.md) | Вычислить первое главное направление в точке по параметрам |
|  | [PrincipalDirection2](M_TFlex_Model_Model3D_Geometry_BaseSurface_PrincipalDirection2.md) | Вычислить второе главное направление в точке по параметрам |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)