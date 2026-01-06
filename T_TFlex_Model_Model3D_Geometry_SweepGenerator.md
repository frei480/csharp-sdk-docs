

Руководство по T-FLEX CAD Open API

# SweepGenerator - класс  
    
Генератор тела по траектории

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryBaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md) [TFlex.Model.Model3D.GeometryBodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md) TFlex.Model.Model3D.GeometrySweepGenerator

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class SweepGenerator : BodyGenerator, 
	IDisposable
```




Тип SweepGenerator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [SweepGenerator](M_TFlex_Model_Model3D_Geometry_SweepGenerator__ctor.md) | Конструктор для задания тела по траектории |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Alignment](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Alignment.md) | Ориентация контура |
|  | [AllowRationals](P_TFlex_Model_Model3D_Geometry_SweepGenerator_AllowRationals.md) | Параметр построения боковых поверхностей в форме рациональных сплайнов |
|  | [Fair](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Fair.md) | Параметр улучшения формы результирующего тела в случае пространственной траектории |
|  | [Ignorable](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Ignorable.md) | Получить множество игнорируемых вершин траектории. |
|  | [LastResult](P_TFlex_Model_Model3D_Geometry_BaseGenerator_LastResult.md) | Результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [MinimiseTolerance](P_TFlex_Model_Model3D_Geometry_SweepGenerator_MinimiseTolerance.md) | Параметр минимизации точности, где это возможно |
|  | [Proxy](P_TFlex_Model_Model3D_Geometry_BaseGenerator_Proxy.md) | Получить внешнее приложение, для которого генерируется результат(Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Result](P_TFlex_Model_Model3D_Geometry_BodyGenerator_Result.md) | Получить множество результирующих тел(Унаследован от [BodyGenerator](T_TFlex_Model_Model3D_Geometry_BodyGenerator.md)) |
|  | [Scale](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Scale.md) | Получить закон масштабирования |
|  | [ScalePoint](P_TFlex_Model_Model3D_Geometry_SweepGenerator_ScalePoint.md) | Точка масштабирования для способов масштабирования Posn и Size |
|  | [ScaleType](P_TFlex_Model_Model3D_Geometry_SweepGenerator_ScaleType.md) | Способ масштабирования |
|  | [Simplify](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Simplify.md) | Параметр упрощения геометрии |
|  | [Tolerance](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Tolerance.md) | Точность геометрии |
|  | [TopologyForm](P_TFlex_Model_Model3D_Geometry_SweepGenerator_TopologyForm.md) | Тип разбиения |
|  | [Twist](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Twist.md) | Получить закон кручения |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose.md) | (Унаследован от [BaseGenerator](T_TFlex_Model_Model3D_Geometry_BaseGenerator.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом SweepGenerator, а при необходимости освобождает также управляемые ресурсы(Переопределяет [BaseGeneratorDispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Dispose_1.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Run](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Run.md) | Функция генерации тела по траектории(Переопределяет [BaseGeneratorRun](M_TFlex_Model_Model3D_Geometry_BaseGenerator_Run.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)