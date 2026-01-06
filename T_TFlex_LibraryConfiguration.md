

Руководство по T-FLEX CAD Open API

# LibraryConfiguration - класс  
    
Класс конфигурации библиотек. Данный класс является набором библиотек и групп библиотек

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlexLibraryConfiguration

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class LibraryConfiguration : IEnumerable<Library>, 
	IDisposable
```




Тип LibraryConfiguration предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [LibraryConfiguration](M_TFlex_LibraryConfiguration__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Count](P_TFlex_LibraryConfiguration_Count.md) | Количество библиотек |
|  | [GroupsCount](P_TFlex_LibraryConfiguration_GroupsCount.md) | Количество групп |
|  | [Name](P_TFlex_LibraryConfiguration_Name.md) | Имя конфигурации библиотеки |
|  | [Path](P_TFlex_LibraryConfiguration_Path.md) | Путь к конфигурации |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_LibraryConfiguration_Dispose.md) | Освобождает все ресурсы, используемые объектом LibraryConfiguration |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetEnumerator](M_TFlex_LibraryConfiguration_GetEnumerator.md) | Получить перечислитель библиотек |
|  | [GetGroup](M_TFlex_LibraryConfiguration_GetGroup.md) | Получить группу по индексу |
|  | [GetGroups](M_TFlex_LibraryConfiguration_GetGroups.md) | Получить перечислитель групп |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetLibrariesWithoutGroup](M_TFlex_LibraryConfiguration_GetLibrariesWithoutGroup.md) | Получить перечислитель библиотек, не входящих ни в одну группу. |
|  | [GetLibrary](M_TFlex_LibraryConfiguration_GetLibrary.md) | Получить библиотеку по индексу |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Save](M_TFlex_LibraryConfiguration_Save.md) | Сохранить конфигурацию |
|  | [SaveAs](M_TFlex_LibraryConfiguration_SaveAs.md) | Сохранить конфигурацию как |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex - пространство имён](N_TFlex.md)