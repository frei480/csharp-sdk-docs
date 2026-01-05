

Руководство по T-FLEX CAD Open API

# SweepGeneratorLawDiscrete - класс  
  
---  
  
Табличная функция : вершина траектории и значение закона в ней. Возможно перечисление значений с использованием конструкции foreach

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometrySweepGeneratorLawDiscrete

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Discrete : IEnumerator, IEnumerable
```
```vb
Public Class Discrete
	Implements IEnumerator, IEnumerable
```
```cpp
public ref class Discrete : IEnumerator, 
	IEnumerable
```


Тип SweepGeneratorLawDiscrete предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Current](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_Current.md) | Получить текущий элемент |
|  | [Item](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_Item.md) |  |
|  | [Length](P_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_Length.md) | Количество пар |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Add](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_Add.md) | Добавить пару в конец списка |
|  | [Delete](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_Delete.md) | Удалить пару по номеру |
|  | [DeleteAll](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_DeleteAll.md) | Удалить все пары |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_GetEnumerator.md) | Получить перечислитель |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Insert](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_Insert.md) | Вставить пару перед номером |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveNext](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_MoveNext.md) | Перейти к следующему элементу |
|  | [Reset](M_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_Reset.md) | Сбросить перечислитель |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Можно задавать любой набор пар вершина траектории / значение. То есть не обязательно задавать закон во всех точках. Порядок задания пар несущественен за исключением замкнутой траектории. В последнем случае первое вхождение в список вершины ассоциируется с начальным значением функции. Второй вхождение - с конечным значением функции. Существует два специальных варианта интерпретации закона : \- Если в таблице только одна пара, то функция считается константной; \- Если в таблице две пары, соответственно для начальной вершины и конечной вершины траектории, то используется линейная интерполяция.

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)