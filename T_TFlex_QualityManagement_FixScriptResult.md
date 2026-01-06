

Руководство по T-FLEX CAD Open API

# FixScriptResult - класс  
    
Результат исправления сценария, суммирующий результаты исправления отдельных проверок

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.QualityManagementFixScriptResult

**Пространство имён:** [TFlex.QualityManagement](N_TFlex_QualityManagement.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class FixScriptResult : IEnumerable<FixResult>
```




Тип FixScriptResult предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [IsDisposed](P_TFlex_QualityManagement_FixScriptResult_IsDisposed.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_QualityManagement_FixScriptResult_Dispose.md) | Освобождает все ресурсы, используемые объектом FixScriptResult |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_QualityManagement_FixScriptResult_GetEnumerator.md) | Получить перечислитель отдельных результатов исправлений |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [LoadFromFile](M_TFlex_QualityManagement_FixScriptResult_LoadFromFile.md) | Загрузить результат из файла по указанному пути. При ошибке загрузки выбрасывается исключение. |
|  | [SaveToFile](M_TFlex_QualityManagement_FixScriptResult_SaveToFile.md) | Сохранять результат в файл по указанному пути. При ошибке сохранения выбрасывается исключение. |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [TryLoadFromFile](M_TFlex_QualityManagement_FixScriptResult_TryLoadFromFile.md) | Загрузить результат из файла по указанному пути. При ошибке загрузки выбрасывается исключение. |
|  | [TrySaveToFile](M_TFlex_QualityManagement_FixScriptResult_TrySaveToFile.md) | Сохранять результат в файл по указанному пути. При ошибке сохранения возвращается false. |
  
#### Ссылки

[TFlex.QualityManagement - пространство имён](N_TFlex_QualityManagement.md)