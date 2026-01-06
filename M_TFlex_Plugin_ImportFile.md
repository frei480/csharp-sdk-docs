

Руководство по T-FLEX CAD Open API

# PluginImportFile - метод  
    
Приложение переопределяет данный метод для импорта указанного файла

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual Document ImportFile(
	string fileName
)
```
```vb
Protected Overridable Function ImportFile ( 
	fileName As String
) As Document
```
```cpp
protected:
virtual Document^ ImportFile(
	String^ fileName
)
```


#### Параметры

fileName [String](https://learn.microsoft.com/dotnet/api/system.string)
    

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Документ, в который был импортирован указанный файл, либо null, если формат файла не поддерживается данным приложением

| Исключение | Условие |
| --- | --- |
| [OperationCanceledException](https://learn.microsoft.com/dotnet/api/system.operationcanceledexception) | Выбрасывается, если данное приложение поддерживает формат указанного файла, но импорт был отменён пользователем |
  
В отличие от [ShowingImportDialogEventHandler(ShowingImportExportDialogEventArgs)](M_TFlex_Plugin_ShowingImportDialogEventHandler.md) и [ImportDialogShownEventHandler(ImportExportDialogShownEventArgs)](M_TFlex_Plugin_ImportDialogShownEventHandler.md), этот метод вызывается при передаче имён файлов через параметры командной строки или перетаскивании файлов на главное окно T-FLEX CAD.

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)

[ShowingImportDialogEventHandler(ShowingImportExportDialogEventArgs)](M_TFlex_Plugin_ShowingImportDialogEventHandler.md)

[ImportDialogShownEventHandler(ImportExportDialogShownEventArgs)](M_TFlex_Plugin_ImportDialogShownEventHandler.md)