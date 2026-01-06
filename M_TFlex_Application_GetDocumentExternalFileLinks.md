

Руководство по T-FLEX CAD Open API

# ApplicationGetDocumentExternalFileLinks - метод  
    
Возвращает все имеющиеся в модели ссылки на внешние файлы

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static string[] GetDocumentExternalFileLinks(
	string fileName,
	bool includeModelFilesOnly,
	bool includeLibraryLinks,
	bool recursive
)
```




#### Параметры

fileName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя файла документа
includeModelFilesOnly [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
includeLibraryLinks [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
recursive [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[String](https://learn.microsoft.com/dotnet/api/system.string)

#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)