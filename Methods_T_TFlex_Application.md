

Руководство по T-FLEX CAD Open API

# Application - методы  
  
---  
  
Тип [Application](T_TFlex_Application.md) предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDocumentsSearchFolder](M_TFlex_Application_AddDocumentsSearchFolder.md) | Назначить папку для поиска указанного типа файлов, если при работе с системой она не была задана явно |
|  | [AddMacrosIndirectAssembly](M_TFlex_Application_AddMacrosIndirectAssembly.md) | Добавить ссылку на сборку в макрос |
|  | [AddResourceFile(String)](M_TFlex_Application_AddResourceFile.md) | Загружает строковые ресурсы из указанного файла в формате Microsoft ResX для использования в неуправляемом коде |
|  | [AddResourceFile(String, String)](M_TFlex_Application_AddResourceFile_1.md) | Загружает строковые ресурсы из указанного файла в формате Microsoft ResX для использования в неуправляемом коде |
|  | [CallPluginRestService](M_TFlex_Application_CallPluginRestService.md) | Вызвать RESTful сервис плагина. Формат входных/выходных данных зависит от конкретного плагина. |
|  | [CreateAnnotation](M_TFlex_Application_CreateAnnotation.md) | Создать новую аннотацию для указанного файла документа |
|  | [DoEvents](M_TFlex_Application_DoEvents.md) | Обрабатывает все сообщения Windows, которые в данный момент находятся в очереди сообщений. |
|  | [EnableDOCs](M_TFlex_Application_EnableDOCs.md) | Разрешить интеграцию с T-FLEX DOCs |
|  | [EnableNotRespondingDialog](M_TFlex_Application_EnableNotRespondingDialog.md) | Для внутреннего использования |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ExecuteDocumentRequest](M_TFlex_Application_ExecuteDocumentRequest.md) |  |
|  | [ExecuteDocumentRequestFile](M_TFlex_Application_ExecuteDocumentRequestFile.md) |  |
|  | [ExitSession](M_TFlex_Application_ExitSession.md) | Завершить работу c API |
|  | [FindLibraryName](M_TFlex_Application_FindLibraryName.md) | Поиск библиотечного пути |
|  | [FindPathName(String)](M_TFlex_Application_FindPathName.md) | Полный путь к файлу |
|  | [FindPathName(String, String)](M_TFlex_Application_FindPathName_1.md) | Полный путь к файлу |
|  | [ForceCulture](M_TFlex_Application_ForceCulture.md) | Принудительно выставить локализацию текущему потому. Использовать в using-e. |
|  | [GetCustomLicenseStatus](M_TFlex_Application_GetCustomLicenseStatus.md) | Получить статус лицензии пользователя |
|  | [GetDocumentExternalFileLinks](M_TFlex_Application_GetDocumentExternalFileLinks.md) | Возвращает все имеющиеся в модели ссылки на внешние файлы |
|  | [GetDocumentIcon(String)](M_TFlex_Application_GetDocumentIcon.md) | Возвращает иконку документа, если она есть |
|  | [GetDocumentIcon(String, Int32)](M_TFlex_Application_GetDocumentIcon_1.md) | Возвращает иконку документа с указанным размером, если она есть |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetShortPathName](M_TFlex_Application_GetShortPathName.md) | Получение короткого пути относительно папки |
|  | [GetSystemFilePath](M_TFlex_Application_GetSystemFilePath.md) | Полный путь к системному файлу |
|  | [GetSystemProfileFilePath](M_TFlex_Application_GetSystemProfileFilePath.md) | Полный путь к системному файлу |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [HideEmbeddedHelp](M_TFlex_Application_HideEmbeddedHelp.md) | Убрать раздел справочного руководства |
|  | [IdleSession](M_TFlex_Application_IdleSession.md) | Для внутреннего использования |
|  | [InitializeCustomLicense](M_TFlex_Application_InitializeCustomLicense.md) | Активировать лицензию пользователя |
|  | [InitSession](M_TFlex_Application_InitSession.md) | Инициализация API |
|  | [LockUpdateUI](M_TFlex_Application_LockUpdateUI.md) | Создать блокировщик обновления интерфейса |
|  | [NewAnnotation](M_TFlex_Application_NewAnnotation.md) | Создать новую аннотацию для указанного файла документа |
|  | [NewDocument](M_TFlex_Application_NewDocument.md) | Создать новый документ |
|  | [NewDocument(Boolean)](M_TFlex_Application_NewDocument_1.md) | Создать новый документ |
|  | [NewDocument(String)](M_TFlex_Application_NewDocument_3.md) | Создать новый документ на основе указанного файла прототипа |
|  | [NewDocument(Boolean, Boolean)](M_TFlex_Application_NewDocument_2.md) | Создать новый документ |
|  | [NewDocument(String, Boolean)](M_TFlex_Application_NewDocument_4.md) | Создать новый документ на основе указанного файла прототипа |
|  | [OpenAsDocument(String)](M_TFlex_Application_OpenAsDocument.md) | Открыть документ или импортировать файл |
|  | [OpenAsDocument(String, Boolean)](M_TFlex_Application_OpenAsDocument_1.md) | Открыть документ или импортировать файл |
|  | [OpenAsDocument(String, Boolean, Boolean)](M_TFlex_Application_OpenAsDocument_2.md) | Открыть документ или импортировать файл |
|  | [OpenDocument(FileLink)](M_TFlex_Application_OpenDocument_4.md) | Открыть документ |
|  | [OpenDocument(String)](M_TFlex_Application_OpenDocument.md) | Открыть документ |
|  | [OpenDocument(FileLink, Boolean)](M_TFlex_Application_OpenDocument_5.md) | Открыть документ |
|  | [OpenDocument(String, Boolean)](M_TFlex_Application_OpenDocument_1.md) | Открыть документ |
|  | [OpenDocument(String, OpenDocumentOptions)](M_TFlex_Application_OpenDocument_3.md) | Открыть документ |
|  | [OpenDocument(FileLink, Boolean, Boolean)](M_TFlex_Application_OpenDocument_6.md) | Открыть документ |
|  | [OpenDocument(String, Boolean, Boolean)](M_TFlex_Application_OpenDocument_2.md) | Открыть документ |
|  | [OpenDocumentFromDOCs(Guid, OpenDocumentOptions)](M_TFlex_Application_OpenDocumentFromDOCs.md) |  |
|  | [OpenDocumentFromDOCs(Int32, Boolean)](M_TFlex_Application_OpenDocumentFromDOCs_1.md) | **Устарело.** T-FLEX DOCs 11 больше не поддерживается |
|  | [OpenDocumentFromDOCs(Int32, Boolean, Boolean)](M_TFlex_Application_OpenDocumentFromDOCs_2.md) | **Устарело.** T-FLEX DOCs 11 больше не поддерживается |
|  | [OpenFileDialog](M_TFlex_Application_OpenFileDialog.md) | Диалог выбора файла из папки или библиотеки |
|  | [OpenFragmentDocument(FileLink)](M_TFlex_Application_OpenFragmentDocument_2.md) | Открыть документ фрагмента для чтения |
|  | [OpenFragmentDocument(String)](M_TFlex_Application_OpenFragmentDocument.md) | Открыть документ фрагмента для чтения |
|  | [OpenFragmentDocument(FileLink, Boolean, Boolean)](M_TFlex_Application_OpenFragmentDocument_3.md) | Открыть документ фрагмента для чтения |
|  | [OpenFragmentDocument(String, Boolean, Boolean)](M_TFlex_Application_OpenFragmentDocument_1.md) | Открыть документ фрагмента для чтения |
|  | [PickPoint(PickPointParameters)](M_TFlex_Application_PickPoint_1.md) | Получить точку в одном из видов активного документа |
|  | [PickPoint(Document, PickPointParameters)](M_TFlex_Application_PickPoint.md) | Получить точку в одном из видов документа |
|  | [RunSystemCommand](M_TFlex_Application_RunSystemCommand.md) | Выполнить команду с ожиданием её завершения |
|  | [ShowEmbeddedHelpTopic](M_TFlex_Application_ShowEmbeddedHelpTopic.md) | Показать раздел справочного руководства |
|  | [ShowHelp](M_TFlex_Application_ShowHelp.md) | Показать справочное руководство |
|  | [TerminateAllCommands](M_TFlex_Application_TerminateAllCommands.md) | Завершить все активные комманды |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [WaitForSystemCommandFinished](M_TFlex_Application_WaitForSystemCommandFinished.md) | Ожидание завершения команды |
  
#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)