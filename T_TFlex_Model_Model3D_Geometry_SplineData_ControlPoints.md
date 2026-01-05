

Руководство по T-FLEX CAD Open API

# SplineDataControlPoints - класс  
  
---  
  
Класс представляет упорядоченное множество контрольных точек - координат точки и вес, если используется

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometrySplineDataControlPoints

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class ControlPoints : IEnumerator, 
	IEnumerable
```
```vb
Public Class ControlPoints
	Implements IEnumerator, IEnumerable
```
```cpp
public ref class ControlPoints : IEnumerator, 
	IEnumerable
```


Тип SplineDataControlPoints предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Current](P_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_Current.md) | Получить текущий элемент |
|  | [Item](P_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_Item.md) |  |
|  | [Length](P_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_Length.md) | Количество контрольных точек |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Add](M_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_Add.md) | Добавить контрольную точку в конец списка |
|  | [Delete](M_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_Delete.md) | Удалить контрольную точку по номеру |
|  | [DeleteAll](M_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_DeleteAll.md) | Удалить все контрольные точки |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_GetEnumerator.md) | Получить перечислитель |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Insert](M_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_Insert.md) | Вставить контрольную точку перед номером |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveNext](M_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_MoveNext.md) | Перейти к следующему элементу |
|  | [Reset](M_TFlex_Model_Model3D_Geometry_SplineData_ControlPoints_Reset.md) | Сбросить перечислитель |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Возможно перечисление точек с использованием конструкции foreach

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)