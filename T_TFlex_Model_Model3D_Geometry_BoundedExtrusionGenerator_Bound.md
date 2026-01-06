

Руководство по T-FLEX CAD Open API

# BoundedExtrusionGeneratorBound - класс  
    
Класс задания границы

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometryBoundedExtrusionGeneratorBound

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Bound : ICloneable, IDisposable
```
```vb
Public Class Bound
	Implements ICloneable, IDisposable
```
```cpp
public ref class Bound : ICloneable, IDisposable
```


Тип BoundedExtrusionGeneratorBound предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BoundedExtrusionGeneratorBound(Boolean, Double)](M_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound__ctor.md) | Конструктор для задания границы значением отступа |
|  | [BoundedExtrusionGeneratorBound(Boolean, BaseBody, Boolean, UInt32, BoundedExtrusionGeneratorBoundSideType)](M_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound__ctor_1.md) | Конструктор для задания границы телом |
|  | [BoundedExtrusionGeneratorBound(Boolean, BaseFace, Boolean, UInt32, BoundedExtrusionGeneratorBoundSideType)](M_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound__ctor_2.md) | Конструктор для задания границы гранью |
|  | [BoundedExtrusionGeneratorBound(Boolean, BaseSurface, Boolean, UInt32, BoundedExtrusionGeneratorBoundSideType)](M_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound__ctor_3.md) | Конструктор для задания границы поверхностью |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [BoundBody](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_BoundBody.md) | Граничное тело |
|  | [BoundDistance](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_BoundDistance.md) | Значение отступа |
|  | [BoundFace](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_BoundFace.md) | Граничная грань |
|  | [BoundSurface](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_BoundSurface.md) | Граничная поверхность |
|  | [BoundType](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_BoundType.md) | Тип границы |
|  | [Division](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_Division.md) | Номер разбиения. Разбиения нумеруются от 1 |
|  | [Forward](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_Forward.md) | Граница задаётся в направлении вектора выталкивания ( true ) или в обратном направлении ( false ) |
|  | [Nearest](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_Nearest.md) | Если true, то разбиения нумеруются начиная с первого и увеличиваясь в направлении движения от профиля. Если false, то первое разбиение наиболее удалено от профиля и номер разбиения увеличивается в направлении движения к профилю. |
|  | [Side](P_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_Side.md) | Какая сторона ограничивающего тела, пересекающая профиль, считается первым разбиением |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_Clone.md) |  |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_Dispose.md) | Освобождает все ресурсы, используемые объектом BoundedExtrusionGeneratorBound |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом BoundedExtrusionGeneratorBound, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Граница может задаваться четырьмя взаимоисключающими способами : листовым или твёрдым телом, гранью, поверхностью, отступом

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)