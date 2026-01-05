

Руководство по T-FLEX CAD Open API

# SurfaceSplineDataControlNet - класс  
  
---  
  
Сетка контрольных точек

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometrySurfaceSplineDataControlNet

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class ControlNet : IEnumerator, IEnumerable
```
```vb
Public Class ControlNet
	Implements IEnumerator, IEnumerable
```
```cpp
public ref class ControlNet : IEnumerator, 
	IEnumerable
```


Тип SurfaceSplineDataControlNet предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Current](P_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_Current.md) | Получить текущий элемент |
|  | [Item](P_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_Item.md) |  |
|  | [ULength](P_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_ULength.md) | Количество строк. Количество изопараметрических кривых по U |
|  | [VLength](P_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_VLength.md) | Количество столбцов. Количество изопараметрических кривых по V |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [DeleteAll](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_DeleteAll.md) | Удалить все контрольные точки |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_GetEnumerator.md) | Получить перечислитель |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveNext](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_MoveNext.md) | Перейти к следующему элементу |
|  | [Reset](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_Reset.md) | Сбросить перечислитель |
|  | [SetSize](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_SetSize.md) | Задать размер решётки |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [UAdd](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_UAdd.md) | Добавить строку в конец сетки. Добавить новую изопараметрическую кривую по U с большим значением U |
|  | [UDelete](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_UDelete.md) | Удалить строку. Удалить изопараметрическую кривую по U |
|  | [UInsert](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_UInsert.md) | Вставить строку. Вставить изопараметрическую кривую по U |
|  | [VAdd](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_VAdd.md) | Добавить столбец в конец сетки. Добавить новую изопараметрическую кривую по V с большим значением V |
|  | [VDelete](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_VDelete.md) | Удалить столбец. Удалить изопараметрическую кривую по V |
|  | [VInsert](M_TFlex_Model_Model3D_Geometry_SurfaceSplineData_ControlNet_VInsert.md) | Вставить столбец. Вставить изопараметрическую кривую по V |
  
Каждая строка соответствует изопараметрической кривой по U. Возможно перечисление строк с использованием конструкции foreach

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)