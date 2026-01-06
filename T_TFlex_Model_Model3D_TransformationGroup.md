

Руководство по T-FLEX CAD Open API

# TransformationGroup - класс  
    
Группа трансформаций

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3DTransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md) TFlex.Model.Model3DTransformationGroup

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class TransformationGroup : TransformationGroupBase
```
```vb
Public Class TransformationGroup
	Inherits TransformationGroupBase
```
```cpp
public ref class TransformationGroup : public TransformationGroupBase
```


Тип TransformationGroup предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [IndexInContainer](P_TFlex_Model_Model3D_TransformationGroup_IndexInContainer.md) | Индекс группы трансформации в контейнере |
|  | [IsValid](P_TFlex_Model_Model3D_TransformationGroupBase_IsValid.md) | true - группа трансформаций все еще находится в контейнере трансформаций. false - объект устарел. Использование приведет к исключениям.(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [Name](P_TFlex_Model_Model3D_TransformationGroupBase_Name.md) | Имя группы(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [Suppressed](P_TFlex_Model_Model3D_TransformationGroupBase_Suppressed.md) | Параметр подавления группы трансформаций. Если больше 0 - группа подавлена.(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [TransfContainer](P_TFlex_Model_Model3D_TransformationGroupBase_TransfContainer.md) | Контейнер групп трансформаций, которому принадлежит данная группа(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDirectAxisByAxisToDirectionTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddDirectAxisByAxisToDirectionTransf.md) | Добавить трансформацию "Повернуть ось вокруг оси по направлению" к группе трансформаций.(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddDirectAxisByAxisToPointTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddDirectAxisByAxisToPointTransf.md) | Добавить трансформацию "Повернуть ось вокруг оси по направлению к точке" к группе трансформаций.(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddDirectAxisToPointTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddDirectAxisToPointTransf.md) | Добавить трансформацию "Направить ось на точку" к группе трансформаций.(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddMap](M_TFlex_Model_Model3D_TransformationGroupBase_AddMap.md) | Добавить матрицу преобразований к группе трансформаций(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddMoveToCurveTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveToCurveTransf.md) | Добавить трансформацию "Перемещение до кривой" к группе трансформаций(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddMoveToNodeTransf(ModelPoint3D)](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveToNodeTransf.md) | Добавить трансформации "Перемещение до точки" к группе трансформаций. Трансформации добавляются для всех осей.(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddMoveToNodeTransf(TransformationCoordinate, ModelPoint3D)](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveToNodeTransf_1.md) | Добавить трансформацию "Перемещение до точки" к группе трансформаций(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddMoveToSurfaceTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveToSurfaceTransf.md) | Добавить трансформацию "Перемещение до плоскости" к группе трансформаций(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddMoveTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddMoveTransf.md) | Добавить трансформацию "Перемещение" к группе трансформаций(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddRotateTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddRotateTransf.md) | Добавить трансформацию "Вращение" к группе трансформаций(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddSetAxisDirectionTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddSetAxisDirectionTransf.md) | Добавить трансформацию "Повернуть параллельно направлению" к группе трансформаций.(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [AddSetAxisTransf](M_TFlex_Model_Model3D_TransformationGroupBase_AddSetAxisTransf.md) | Добавить трансформацию "Совместить ось полностью" к группе трансформаций.(Унаследован от [TransformationGroupBase](T_TFlex_Model_Model3D_TransformationGroupBase.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetLCS](M_TFlex_Model_Model3D_TransformationGroup_GetLCS.md) | Получить ЛСК группы трансформации |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [SetLCS](M_TFlex_Model_Model3D_TransformationGroup_SetLCS.md) | Задать ЛСК группы трансформации |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)