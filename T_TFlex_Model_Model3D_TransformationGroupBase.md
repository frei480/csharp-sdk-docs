

Руководство по T-FLEX CAD Open API

# TransformationGroupBase - класс  
    
Базовый класс групп трансформаций

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3DTransformationGroupBase [TFlex.Model.Model3DTransformationGroup](T_TFlex_Model_Model3D_TransformationGroup.md)

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class TransformationGroupBase
```
```vb
Public MustInherit Class TransformationGroupBase
```
```cpp
public ref class TransformationGroupBase abstract
```


Тип TransformationGroupBase предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [IsValid](P_TFlex_Model_Model3D_TransformationGroupBase_IsValid.md) | true - группа трансформаций все еще находится в контейнере трансформаций. false - объект устарел. Использование приведет к исключениям. |
|  | [Name](P_TFlex_Model_Model3D_TransformationGroupBase_Name.md) | Имя группы |
|  | [Suppressed](P_TFlex_Model_Model3D_TransformationGroupBase_Suppressed.md) | Параметр подавления группы трансформаций. Если больше 0 - группа подавлена. |
|  | [TransfContainer](P_TFlex_Model_Model3D_TransformationGroupBase_TransfContainer.md) | Контейнер групп трансформаций, которому принадлежит данная группа |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDirectAxisByAxisToDirectionTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddDirectAxisByAxisToDirectionTransf.md) | Добавить трансформацию "Повернуть ось вокруг оси по направлению" к группе трансформаций. |
|  | [AddDirectAxisByAxisToPointTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddDirectAxisByAxisToPointTransf.md) | Добавить трансформацию "Повернуть ось вокруг оси по направлению к точке" к группе трансформаций. |
|  | [AddDirectAxisToPointTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddDirectAxisToPointTransf.md) | Добавить трансформацию "Направить ось на точку" к группе трансформаций. |
|  | [AddMap](M_TFlex_Model_Model3D_TransformationGroupBase_AddMap.md) | Добавить матрицу преобразований к группе трансформаций |
|  | [AddMoveToCurveTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveToCurveTransf.md) | Добавить трансформацию "Перемещение до кривой" к группе трансформаций |
|  | [AddMoveToNodeTransf(ModelPoint3D)](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveToNodeTransf.md) | Добавить трансформации "Перемещение до точки" к группе трансформаций. Трансформации добавляются для всех осей. |
|  | [AddMoveToNodeTransf(TransformationCoordinate, ModelPoint3D)](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveToNodeTransf_1.md) | Добавить трансформацию "Перемещение до точки" к группе трансформаций |
|  | [AddMoveToSurfaceTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveToSurfaceTransf.md) | Добавить трансформацию "Перемещение до плоскости" к группе трансформаций |
|  | [AddMoveTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveTransf.md) | Добавить трансформацию "Перемещение" к группе трансформаций |
|  | [AddRotateTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddRotateTransf.md) | Добавить трансформацию "Вращение" к группе трансформаций |
|  | [AddSetAxisDirectionTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddSetAxisDirectionTransf.md) | Добавить трансформацию "Повернуть параллельно направлению" к группе трансформаций. |
|  | [AddSetAxisTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddSetAxisTransf.md) | Добавить трансформацию "Совместить ось полностью" к группе трансформаций. |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)