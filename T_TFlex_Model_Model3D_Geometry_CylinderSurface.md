

Руководство по T-FLEX CAD Open API

# CylinderSurface - класс  
    
Геометрический цилиндр

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) [TFlex.Model.Model3D.GeometryBaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md) [TFlex.Model.Model3D.GeometrySurface](T_TFlex_Model_Model3D_Geometry_Surface.md) TFlex.Model.Model3D.GeometryCylinderSurface

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class CylinderSurface : Surface, 
	BaseCylinderSurface
```
```vb
Public Class CylinderSurface
	Inherits Surface
	Implements BaseCylinderSurface
```
```cpp
public ref class CylinderSurface : public Surface, 
	BaseCylinderSurface
```


Тип CylinderSurface предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [CylinderSurface](M_TFlex_Model_Model3D_Geometry_CylinderSurface__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Axis](P_TFlex_Model_Model3D_Geometry_CylinderSurface_Axis.md) | Получить ось симметрии |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [ParasolidSurface](P_TFlex_Model_Model3D_Geometry_BaseSurface_ParasolidSurface.md) | (Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [Radius](P_TFlex_Model_Model3D_Geometry_CylinderSurface_Radius.md) | Радиус основания |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [ReferenceDirection](P_TFlex_Model_Model3D_Geometry_CylinderSurface_ReferenceDirection.md) | Полуось основания, от которой откладывается угол |
|  | [UParam](P_TFlex_Model_Model3D_Geometry_BaseSurface_UParam.md) | Получить информацию о параметризации по U(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [VParam](P_TFlex_Model_Model3D_Geometry_BaseSurface_VParam.md) | Получить информацию о параметризации по V(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ApplyTransform](M_TFlex_Model_Model3D_Geometry_BaseSurface_ApplyTransform.md) | Трансформация поверхности(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [Derivative](M_TFlex_Model_Model3D_Geometry_BaseSurface_Derivative.md) | Вычислить производные в точке на поверхности по параметрам(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseSurface_Dispose.md) | (Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Eval](M_TFlex_Model_Model3D_Geometry_BaseSurface_Eval.md) | Вычислить координаты точки на поверхности по параметрам(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_BaseSurface_Finalize.md) | (Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IntersectCurve](M_TFlex_Model_Model3D_Geometry_BaseSurface_IntersectCurve.md) | Найти пересечение поверхности с кривой(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [IntersectSurface](M_TFlex_Model_Model3D_Geometry_BaseSurface_IntersectSurface.md) | Найти пересечение поверхности с другой поверхностью(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Normal](M_TFlex_Model_Model3D_Geometry_BaseSurface_Normal.md) | Вычислить нормаль к поверхности в точке по параметрам(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [Parameterize](M_TFlex_Model_Model3D_Geometry_BaseSurface_Parameterize.md) | Вычислить параметр на поверхности, для точки, лежащей на поверхности(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [Parameterize2](M_TFlex_Model_Model3D_Geometry_BaseSurface_Parameterize2.md) | Вычислить параметры на поверхности, для точки, лежащей около нее(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [PrincipalCurvature1](M_TFlex_Model_Model3D_Geometry_BaseSurface_PrincipalCurvature1.md) | Вычислить первую главную кривизну в точек на поверхности по параметрам(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [PrincipalCurvature2](M_TFlex_Model_Model3D_Geometry_BaseSurface_PrincipalCurvature2.md) | Вычислить вторую главную кривизну в точках на поверхности по параметрам(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [PrincipalDirection1](M_TFlex_Model_Model3D_Geometry_BaseSurface_PrincipalDirection1.md) | Вычислить первое главное направление в точке по параметрам(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [PrincipalDirection2](M_TFlex_Model_Model3D_Geometry_BaseSurface_PrincipalDirection2.md) | Вычислить второе главное направление в точке по параметрам(Унаследован от [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)