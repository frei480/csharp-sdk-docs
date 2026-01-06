

Руководство по T-FLEX CAD Open API

# TranslationManipulator - класс  
    
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.Visual.ManipulatorsManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md) TFlex.Model.Model3D.Visual.ManipulatorsTranslationManipulator

**Пространство имён:** [TFlex.Model.Model3D.Visual.Manipulators](N_TFlex_Model_Model3D_Visual_Manipulators.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class TranslationManipulator : Manipulator
```
```vb
Public Class TranslationManipulator
	Inherits Manipulator
```
```cpp
public ref class TranslationManipulator : public Manipulator
```


Тип TranslationManipulator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [TranslationManipulator](M_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator__ctor.md) | Инициализирует новый экземпляр класса TranslationManipulator |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Color](P_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_Color.md) |  |
|  | [IsModelSized](P_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_IsModelSized.md) |  |
|  | [ModelSize](P_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_ModelSize.md) | в модельных единицах (миллиметры, дюймы) |
|  | [UseDynamicEditor](P_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_UseDynamicEditor.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Visible](P_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Visible.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CommitModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CommitModification.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [CreateElems](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CreateElems.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [CreateGeom](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CreateGeom.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Dispose.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом TranslationManipulator, а при необходимости освобождает также управляемые ресурсы(Переопределяет [ManipulatorDispose(Boolean)](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Dispose_1.md)) |
|  | [EnqueueModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_EnqueueModification.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetCommitedGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetCommitedGeometry.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [GetCommitedOffset](M_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_GetCommitedOffset.md) | Получить фиксированное значение смещения в модельных единицах |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetPendingGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetPendingGeometry.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [GetPendingModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetPendingModification.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [GetPendingOffset](M_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_GetPendingOffset.md) | Получить динамическое значение смещения в модельных единицах |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Init](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Init.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Release](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Release.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ResetGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ResetGeometry.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ResetOffset](M_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_ResetOffset.md) | Перезадать смещение в модельных единицах |
|  | [SetAxis](M_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_SetAxis.md) | Задать ось |
|  | [SetParentObject](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_SetParentObject.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CommitedGeometryChanged](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CommitedGeometryChanged.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [EndDrag](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_EndDrag.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ModificationCommited](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ModificationCommited.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ModificationEnqueued](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ModificationEnqueued.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [OffsetCommited](E_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_OffsetCommited.md) |  |
|  | [OffsetEnqueued](E_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator_OffsetEnqueued.md) |  |
|  | [PendingGeometryChanged](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_PendingGeometryChanged.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
  
#### Ссылки

[TFlex.Model.Model3D.Visual.Manipulators - пространство имён](N_TFlex_Model_Model3D_Visual_Manipulators.md)