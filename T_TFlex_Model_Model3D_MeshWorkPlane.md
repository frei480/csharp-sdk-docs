

Руководство по T-FLEX CAD Open API

# MeshWorkPlane - класс  
    
Сетка из точек пересечения рабочих плоскостей

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3DMeshWorkPlane

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class MeshWorkPlane
```
```vb
Public NotInheritable Class MeshWorkPlane
```
```cpp
public ref class MeshWorkPlane sealed
```


Тип MeshWorkPlane предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [MeshWorkPlane](M_TFlex_Model_Model3D_MeshWorkPlane__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ActiveWorkplane](P_TFlex_Model_Model3D_MeshWorkPlane_ActiveWorkplane.md) | Активная рабочая плоскость |
|  | [Enable](P_TFlex_Model_Model3D_MeshWorkPlane_Enable.md) | Включение сетки рабочих плоскостей |
|  | [FindNearPoint](P_TFlex_Model_Model3D_MeshWorkPlane_FindNearPoint.md) | Режим выбора ближайших к лучу точек |
|  | [Inverse](P_TFlex_Model_Model3D_MeshWorkPlane_Inverse.md) | Инверсия порядка возвращаемых узлов сетки, от дальних к ближним |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Build](M_TFlex_Model_Model3D_MeshWorkPlane_Build.md) | Обновление сетки |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindBoundBox](M_TFlex_Model_Model3D_MeshWorkPlane_FindBoundBox.md) | Границы множества точек пересечений рабочих плоскостей |
|  | [FindByCoords](M_TFlex_Model_Model3D_MeshWorkPlane_FindByCoords.md) | Найти точку по её координатам |
|  | [FindFar](M_TFlex_Model_Model3D_MeshWorkPlane_FindFar.md) | Найти удалённую точку по направлению |
|  | [FindMinMax](M_TFlex_Model_Model3D_MeshWorkPlane_FindMinMax.md) | Найти минимальную или максимальную точку на луче |
|  | [FindNear](M_TFlex_Model_Model3D_MeshWorkPlane_FindNear.md) | Найти ближайшую точку по направлению |
|  | [FindNearByLength](M_TFlex_Model_Model3D_MeshWorkPlane_FindNearByLength.md) | Найти ближайшую точку с учётом длины вектора, задающего направление, включая точку на луче |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)