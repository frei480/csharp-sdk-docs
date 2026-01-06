

Руководство по T-FLEX CAD Open API

# TransformationGroupContainer - класс  
    
Контейнер групп трансформаций.

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3DTransformationGroupContainer

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class TransformationGroupContainer
```
```vb
Public Class TransformationGroupContainer
```
```cpp
public ref class TransformationGroupContainer
```


Тип TransformationGroupContainer предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Owner](P_TFlex_Model_Model3D_TransformationGroupContainer_Owner.md) | Объект, которому принадлежит контейнер. |
|  | [SourceCSType](P_TFlex_Model_Model3D_TransformationGroupContainer_SourceCSType.md) | Тип исходной системы координат преобразования |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddBaseTransfGroup](M_TFlex_Model_Model3D_TransformationGroupContainer_AddBaseTransfGroup.md) | Добавить новую группу базовых трансформаций в конец контейнера. |
|  | [CopyTo](M_TFlex_Model_Model3D_TransformationGroupContainer_CopyTo.md) |  |
|  | [DeleteAllBaseTransfGroups](M_TFlex_Model_Model3D_TransformationGroupContainer_DeleteAllBaseTransfGroups.md) | Удалить все группы базовых трансформаций из контейнера. |
|  | [DeleteBaseTransfGroup](M_TFlex_Model_Model3D_TransformationGroupContainer_DeleteBaseTransfGroup.md) | Удалить группу базовых трансформаций из контейнера. |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetBaseTransfCount](M_TFlex_Model_Model3D_TransformationGroupContainer_GetBaseTransfCount.md) | Получить общее число базовых трансформаций в контейнере. |
|  | [GetBaseTransfGroupAt](M_TFlex_Model_Model3D_TransformationGroupContainer_GetBaseTransfGroupAt.md) | Получить группу базовых трансформаций в контейнере с индексом index. |
|  | [GetBaseTransfGroups](M_TFlex_Model_Model3D_TransformationGroupContainer_GetBaseTransfGroups.md) | Получить список всех групп базовых трансформаций в контейнере. |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MakeNonAssociative](M_TFlex_Model_Model3D_TransformationGroupContainer_MakeNonAssociative.md) | Заменить все преобразования одним неассоциативным преобразованием |
|  | [MakeNoneAssociative](M_TFlex_Model_Model3D_TransformationGroupContainer_MakeNoneAssociative.md) | **Устарело.** Заменить все преобразования одним неассоциативным преобразованием |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveBaseTransfGroupDown](M_TFlex_Model_Model3D_TransformationGroupContainer_MoveBaseTransfGroupDown.md) | Переместить базовую группу трансформаций на 1 позицию вниз. В случае успеха transfGroup становится устаревшей (IsValid == false). |
|  | [MoveBaseTransfGroupUp](M_TFlex_Model_Model3D_TransformationGroupContainer_MoveBaseTransfGroupUp.md) | Переместить базовую группу трансформаций на 1 позицию вверх. В случае успеха transfGroup становится устаревшей (IsValid == false). |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)