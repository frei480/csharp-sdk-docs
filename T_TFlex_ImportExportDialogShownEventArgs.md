

Руководство по T-FLEX CAD Open API

# ImportExportDialogShownEventArgs - класс  
  
---  
  
Класс, содержащий данные о событии, возникающем когда диалог импорта или экспорта открыт

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlexPluginEventArgs](T_TFlex_PluginEventArgs.md) [TFlexDocumentEventArgs](T_TFlex_DocumentEventArgs.md) TFlexImportExportDialogShownEventArgs

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class ImportExportDialogShownEventArgs : DocumentEventArgs
```
```vb
Public Class ImportExportDialogShownEventArgs
	Inherits DocumentEventArgs
```
```cpp
public ref class ImportExportDialogShownEventArgs : public DocumentEventArgs
```


Тип ImportExportDialogShownEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Cancel](P_TFlex_PluginEventArgs_Cancel.md) | true, если действие было отменено пользователем или системой(Унаследован от [PluginEventArgs](T_TFlex_PluginEventArgs.md)) |
|  | [Document](P_TFlex_DocumentEventArgs_Document.md) | Документ, в котором произошло данное событие(Унаследован от [DocumentEventArgs](T_TFlex_DocumentEventArgs.md)) |
|  | [FilePath](P_TFlex_ImportExportDialogShownEventArgs_FilePath.md) | Получить имя импортируемого или экспортируемого файла |
|  | [FileterID](P_TFlex_ImportExportDialogShownEventArgs_FileterID.md) | **Устарело.** |
|  | [FilterId](P_TFlex_ImportExportDialogShownEventArgs_FilterId.md) | Получить идентификатор фильтра импортируемого или экспортируемого файла |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [SetImportedDocument](M_TFlex_ImportExportDialogShownEventArgs_SetImportedDocument.md) |  |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex - пространство имён](N_TFlex.md)