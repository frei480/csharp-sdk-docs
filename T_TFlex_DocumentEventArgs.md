

Руководство по T-FLEX CAD Open API

# DocumentEventArgs - класс  
    
Класс, содержащий данные о событии, возникшем в документе

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlexPluginEventArgs](T_TFlex_PluginEventArgs.md) TFlexDocumentEventArgs Подробнее

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class DocumentEventArgs : PluginEventArgs
```




Тип DocumentEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Cancel](P_TFlex_PluginEventArgs_Cancel.md) | true, если действие было отменено пользователем или системой(Унаследован от [PluginEventArgs](T_TFlex_PluginEventArgs.md)) |
|  | [Document](P_TFlex_DocumentEventArgs_Document.md) | Документ, в котором произошло данное событие |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex - пространство имён](N_TFlex.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlexPluginEventArgs](T_TFlex_PluginEventArgs.md) TFlexDocumentEventArgs [TFlexBlockChangesEventArgs](T_TFlex_BlockChangesEventArgs.md) [TFlexCommandEventArgs](T_TFlex_CommandEventArgs.md) [TFlexCopyPropertiesCommandEventArgs](T_TFlex_CopyPropertiesCommandEventArgs.md) [TFlexDynamicAnalysisEventArgs](T_TFlex_DynamicAnalysisEventArgs.md) [TFlexFullRegenerationEventArgs](T_TFlex_FullRegenerationEventArgs.md) [TFlexImportExportDialogShownEventArgs](T_TFlex_ImportExportDialogShownEventArgs.md) [TFlexMeasureResultsUpdatingEventArgs](T_TFlex_MeasureResultsUpdatingEventArgs.md) [TFlexModelConfigurationEventArgs](T_TFlex_ModelConfigurationEventArgs.md) [TFlexObjectEventArgs](T_TFlex_ObjectEventArgs.md) [TFlexObjectsMeasuredEventArgs](T_TFlex_ObjectsMeasuredEventArgs.md) [TFlexPlaneCreateEventArgs](T_TFlex_PlaneCreateEventArgs.md) [TFlexPluginCommandEventArgs](T_TFlex_PluginCommandEventArgs.md) [TFlexRegenerateDocumentEventArgs](T_TFlex_RegenerateDocumentEventArgs.md) [TFlexShowingFullRegenerationDialogEventArgs](T_TFlex_ShowingFullRegenerationDialogEventArgs.md) [TFlexShowingImportExportDialogEventArgs](T_TFlex_ShowingImportExportDialogEventArgs.md) [TFlexTrackingContextPopupMenuEventArgs](T_TFlex_TrackingContextPopupMenuEventArgs.md) [TFlexViewEventArgs](T_TFlex_ViewEventArgs.md) [TFlexViewRulerContextMenuCommandEventArgs](T_TFlex_ViewRulerContextMenuCommandEventArgs.md) [TFlexWorkplaneCommandEventArgs](T_TFlex_WorkplaneCommandEventArgs.md)