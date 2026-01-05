

Руководство по T-FLEX CAD Open API

# GeometricArray - класс  
  
---  
  
Множество геометрических данных

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometryGeometricArray [TFlex.Model.Model3D.GeometryContoursArray](T_TFlex_Model_Model3D_Geometry_ContoursArray.md) [TFlex.Model.Model3D.GeometryPointsArray](T_TFlex_Model_Model3D_Geometry_PointsArray.md) [TFlex.Model.Model3D.GeometrySheetsArray](T_TFlex_Model_Model3D_Geometry_SheetsArray.md) [TFlex.Model.Model3D.GeometryWiresArray](T_TFlex_Model_Model3D_Geometry_WiresArray.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class GeometricArray : IEnumerator, 
	IEnumerable
```
```vb
Public MustInherit Class GeometricArray
	Implements IEnumerator, IEnumerable
```
```cpp
public ref class GeometricArray abstract : IEnumerator, 
	IEnumerable
```


Тип GeometricArray предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Current](P_TFlex_Model_Model3D_Geometry_GeometricArray_Current.md) | Получить текущий элемент |
|  | [Length](P_TFlex_Model_Model3D_Geometry_GeometricArray_Length.md) | Количество элементов |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Add](M_TFlex_Model_Model3D_Geometry_GeometricArray_Add.md) | Добавить элемент в конец списка |
|  | [Delete](M_TFlex_Model_Model3D_Geometry_GeometricArray_Delete.md) | Удалить элемент по номеру |
|  | [DeleteAll](M_TFlex_Model_Model3D_Geometry_GeometricArray_DeleteAll.md) | Удалить все элементы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_Model_Model3D_Geometry_GeometricArray_GetEnumerator.md) | Получить перечислитель |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Insert](M_TFlex_Model_Model3D_Geometry_GeometricArray_Insert.md) | Вставить элемент перед номером |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveNext](M_TFlex_Model_Model3D_Geometry_GeometricArray_MoveNext.md) | Перейти к следующему элементу |
|  | [Reset](M_TFlex_Model_Model3D_Geometry_GeometricArray_Reset.md) | Сбросить перечислитель |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Возможно перечисление элементов с использованием конструкции foreach

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)