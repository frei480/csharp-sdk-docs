

Руководство по T-FLEX CAD Open API

# WireSetManipulator - класс  
  
---  
  
[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.Visual.ManipulatorsManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md) TFlex.Model.Model3D.Visual.ManipulatorsWireSetManipulator [TFlex.Model.Model3D.Visual.ManipulatorsShellWireSetManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_ShellWireSetManipulator.md) [TFlex.Model.Model3D.Visual.ManipulatorsSpliceWireSetManipulator](T_TFlex_Model_Model3D_Visual_Manipulators_SpliceWireSetManipulator.md)

**Пространство имён:** [TFlex.Model.Model3D.Visual.Manipulators](N_TFlex_Model_Model3D_Visual_Manipulators.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class WireSetManipulator : Manipulator
```
```vb
Public Class WireSetManipulator
	Inherits Manipulator
```
```cpp
public ref class WireSetManipulator : public Manipulator
```


Тип WireSetManipulator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [WireSetManipulator](M_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator__ctor.md) | Инициализирует новый экземпляр класса WireSetManipulator |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [IsEditable](P_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_IsEditable.md) |  |
|  | [SelectedPoint](P_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_SelectedPoint.md) |  |
|  | [SelectedSegment](P_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_SelectedSegment.md) |  |
|  | [SelectedTerminalPoint](P_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_SelectedTerminalPoint.md) |  |
|  | [UseDynamicEditor](P_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_UseDynamicEditor.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Visible](P_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Visible.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDisplayedSegment](M_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_AddDisplayedSegment.md) |  |
|  | [CommitModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CommitModification.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [CreateElems](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CreateElems.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [CreateGeom](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CreateGeom.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Dispose.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_Dispose.md) | Освобождает неуправляемые ресурсы, используемые объектом WireSetManipulator, а при необходимости освобождает также управляемые ресурсы(Переопределяет [ManipulatorDispose(Boolean)](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Dispose_1.md)) |
|  | [EnqueueModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_EnqueueModification.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
|  | [GetCommitedGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetCommitedGeometry.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetPendingGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetPendingGeometry.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [GetPendingModification](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_GetPendingModification.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Init](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Init.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Release](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_Release.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ResetDisplayedSegments](M_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_ResetDisplayedSegments.md) |  |
|  | [ResetGeometry](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ResetGeometry.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [Select](M_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_Select.md) |  |
|  | [SetObject](M_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_SetObject.md) |  |
|  | [SetParentObject](M_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_SetParentObject.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CommitedGeometryChanged](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_CommitedGeometryChanged.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [EndDrag](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_EndDrag.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ModificationCommited](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ModificationCommited.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [ModificationEnqueued](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_ModificationEnqueued.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
|  | [OnAddConductors](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnAddConductors.md) |  |
|  | [OnAddOutput](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnAddOutput.md) |  |
|  | [OnAddSleeve](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnAddSleeve.md) |  |
|  | [OnAddSocket](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnAddSocket.md) |  |
|  | [OnChanged](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnChanged.md) |  |
|  | [OnChangeSleeve](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnChangeSleeve.md) |  |
|  | [OnConnectConductors](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnConnectConductors.md) |  |
|  | [OnDeleteSleeve](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnDeleteSleeve.md) |  |
|  | [OnDeleteSplices](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnDeleteSplices.md) |  |
|  | [OnRemoveSocket](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnRemoveSocket.md) |  |
|  | [OnRotateSocket](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnRotateSocket.md) |  |
|  | [OnSelect](E_TFlex_Model_Model3D_Visual_Manipulators_WireSetManipulator_OnSelect.md) |  |
|  | [PendingGeometryChanged](E_TFlex_Model_Model3D_Visual_Manipulators_Manipulator_PendingGeometryChanged.md) | (Унаследован от [Manipulator](T_TFlex_Model_Model3D_Visual_Manipulators_Manipulator.md)) |
  
#### Ссылки

[TFlex.Model.Model3D.Visual.Manipulators - пространство имён](N_TFlex_Model_Model3D_Visual_Manipulators.md)