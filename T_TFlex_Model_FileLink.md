

Руководство по T-FLEX CAD Open API

# FileLink - класс  
    
Класс ссылки на файл

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelFileLink

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class FileLink : IDisposable
```




Тип FileLink предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [FileLink(BackFileLinkParameters)](M_TFlex_Model_FileLink__ctor.md) | Конструктор обратной ссылки |
|  | [FileLink(Document)](M_TFlex_Model_FileLink__ctor_1.md) | Конструктор пустой ссылки на файл |
|  | [FileLink(FileLink)](M_TFlex_Model_FileLink__ctor_7.md) | Конструктор копии ссылки на файл |
|  | [FileLink(TempFileLinkParameters)](M_TFlex_Model_FileLink__ctor_8.md) | Конструктор ссылки на временный файл |
|  | [FileLink(Document, IntPtr)](M_TFlex_Model_FileLink__ctor_2.md) | Конструктор ссылки на файл по внутреннему идентификатору |
|  | [FileLink(Document, String)](M_TFlex_Model_FileLink__ctor_3.md) | Конструктор ссылки на файл по пути |
|  | [FileLink(Document, FileLink)](M_TFlex_Model_FileLink__ctor_6.md) | Конструктор копии ссылки на файл |
|  | [FileLink(Document, String, Boolean)](M_TFlex_Model_FileLink__ctor_4.md) | Конструктор ссылки на внутренний файл по пути |
|  | [FileLink(Document, String, Document)](M_TFlex_Model_FileLink__ctor_5.md) | Конструктор ссылки на внутренний файл по документу в памяти |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Document](P_TFlex_Model_FileLink_Document.md) | Документ объекта |
|  | [FilePath](P_TFlex_Model_FileLink_FilePath.md) | Путь файла |
|  | [FullFilePath](P_TFlex_Model_FileLink_FullFilePath.md) | Полный путь файла |
|  | [InternalID](P_TFlex_Model_FileLink_InternalID.md) | Внутренний идентификатор |
|  | [IsDisposed](P_TFlex_Model_FileLink_IsDisposed.md) | Возвращает true, если вызывался Dispose() |
|  | [IsEmbedded](P_TFlex_Model_FileLink_IsEmbedded.md) | Возвращает true, если ссылка внутренняя |
|  | [IsEmpty](P_TFlex_Model_FileLink_IsEmpty.md) | Возвращает true, если ссылка пустая |
|  | [IsOriginalFormat](P_TFlex_Model_FileLink_IsOriginalFormat.md) | Возвращает true, если ссылка на документ T-FLEX CAD |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_FileLink_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MakeEmbedded](M_TFlex_Model_FileLink_MakeEmbedded.md) | Преобразовать ссылку во вложенную. Будут преобразованы все ссылки в документе на данный файл. |
|  | [MakeExternal](M_TFlex_Model_FileLink_MakeExternal.md) | Преобразовать ссылку во внешнюю. Будут преобразованы все ссылки в документе на данный файл. |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)