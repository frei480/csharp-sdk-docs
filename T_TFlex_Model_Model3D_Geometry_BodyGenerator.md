

Руководство по T-FLEX CAD Open API

# BodyGenerator - класс  
    
Базовый класс для генераторов тел

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryBaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md) TFlex.Model.Model3D.GeometryBodyGenerator Подробнее

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BodyGenerator : BaseGenerator
```




Тип BodyGenerator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BodyGenerator](M_TFlex_Model_Model3D_Geometry_BodyGenerator__ctor.md) | Конструктор для задания генератора |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [LastResult](P_TFlex_Model_Model3D_Geometry_BaseGenerator_LastResult.md) | Результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Proxy](P_TFlex_Model_Model3D_Geometry_BaseGenerator_Proxy.md) | Получить внешнее приложение, для которого генерируется результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Result](P_TFlex_Model_Model3D_Geometry_BodyGenerator_Result.md) | Получить множество результирующих тел |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose.md) | (Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose_1.md) | (Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Run](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Run.md) | Основная функция генерации геометрических результатов(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryBaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md) TFlex.Model.Model3D.GeometryBodyGenerator [TFlex.Model.Model3D.GeometryBooleanGenerator](T_TFlex_Model_Model3D_Geometry_BooleanGenerator.md) [TFlex.Model.Model3D.GeometryBoundedExtrusionGenerator](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator.md) [TFlex.Model.Model3D.GeometryEdgeBlendingGenerator](T_TFlex_Model_Model3D_Geometry_EdgeBlendingGenerator.md) [TFlex.Model.Model3D.GeometryExtrudeGenerator](T_TFlex_Model_Model3D_Geometry_ExtrudeGenerator.md) [TFlex.Model.Model3D.GeometryFaceFaceBlendGenerator](T_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator.md) [TFlex.Model.Model3D.GeometryLoftGenerator](T_TFlex_Model_Model3D_Geometry_LoftGenerator.md) [TFlex.Model.Model3D.GeometryRotateGenerator](T_TFlex_Model_Model3D_Geometry_RotateGenerator.md) [TFlex.Model.Model3D.GeometrySewGenerator](T_TFlex_Model_Model3D_Geometry_SewGenerator.md) [TFlex.Model.Model3D.GeometrySheetFromFaces](T_TFlex_Model_Model3D_Geometry_SheetFromFaces.md) [TFlex.Model.Model3D.GeometrySheetFromTrimmedSurface](T_TFlex_Model_Model3D_Geometry_SheetFromTrimmedSurface.md) [TFlex.Model.Model3D.GeometryShellGenerator](T_TFlex_Model_Model3D_Geometry_ShellGenerator.md) [TFlex.Model.Model3D.GeometrySweepGenerator](T_TFlex_Model_Model3D_Geometry_SweepGenerator.md) [TFlex.Model.Model3D.GeometryThickenExtrusionGenerator](T_TFlex_Model_Model3D_Geometry_ThickenExtrusionGenerator.md) [TFlex.Model.Model3D.GeometryThreeFaceBlendGenerator](T_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator.md) [TFlex.Model.Model3D.GeometryWireFromCurvesGenerator](T_TFlex_Model_Model3D_Geometry_WireFromCurvesGenerator.md) [TFlex.Model.Model3D.GeometryWireFromEdgesGenerator](T_TFlex_Model_Model3D_Geometry_WireFromEdgesGenerator.md)