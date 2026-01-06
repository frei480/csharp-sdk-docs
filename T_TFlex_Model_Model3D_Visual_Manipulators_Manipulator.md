

Руководство по T-FLEX CAD Open API

# Manipulator - класс  
    
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.Visual.ManipulatorsManipulator Подробнее

**Пространство имён:** [TFlex.Model.Model3D.Visual.Manipulators](N_TFlex_Model_Model3D_Visual_Manipulators.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class Manipulator : IDisposable
```




Тип Manipulator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Manipulator](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator__ctor.md) | Инициализирует новый экземпляр класса Manipulator |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [UseDynamicEditor](P_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_UseDynamicEditor.md) |  |
|  | [Visible](P_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Visible.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CommitModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CommitModification.md) |  |
|  | [CreateElems](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CreateElems.md) |  |
|  | [CreateGeom](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CreateGeom.md) |  |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Dispose.md) | Освобождает все ресурсы, используемые объектом Manipulator |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом Manipulator, а при необходимости освобождает также управляемые ресурсы |
|  | [EnqueueModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_EnqueueModification.md) |  |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindPositionOnPath(FloatVector, ModelWire)](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_FindPositionOnPath_1.md) |  |
|  | [FindPositionOnPath(FloatVector, FloatVector, ModelWire)](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_FindPositionOnPath.md) |  |
|  | [GetCommitedGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetCommitedGeometry.md) |  |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetPendingGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetPendingGeometry.md) |  |
|  | [GetPendingModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetPendingModification.md) |  |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Init](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Init.md) |  |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Release](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Release.md) |  |
|  | [ResetGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ResetGeometry.md) |  |
|  | [SetParentObject](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_SetParentObject.md) |  |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CommitedGeometryChanged](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CommitedGeometryChanged.md) |  |
|  | [EndDrag](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_EndDrag.md) |  |
|  | [ModificationCommited](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ModificationCommited.md) |  |
|  | [ModificationEnqueued](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ModificationEnqueued.md) |  |
|  | [PendingGeometryChanged](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_PendingGeometryChanged.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D.Visual.Manipulators - пространство имён](N_TFlex_Model_Model3D_Visual_Manipulators.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.Visual.ManipulatorsManipulator [TFlex.Model.Model3D.Visual.ManipulatorsAngularSizeManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_AngularSizeManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsBoxManipulatorBase](T_TFlex_Model_Model3D_Visual_Manipulators_BoxManipulatorBase.md) [TFlex.Model.Model3D.Visual.ManipulatorsCoordSystemManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_CoordSystemManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsLengthDiameterManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_LengthDiameterManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsLinearSizeManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_LinearSizeManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsObjectTransformManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_ObjectTransformManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsPointOnPathManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_PointOnPathManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsPointRotationManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_PointRotationManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsRotationManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_RotationManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsTranslationManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_TranslationManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsWireManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_WireManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsWireSetManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator.md)