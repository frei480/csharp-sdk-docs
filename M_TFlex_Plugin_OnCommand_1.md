

Руководство по T-FLEX CAD Open API

# PluginOnCommand(Document, Int32) - метод  
    
Приложение переопределяет эту функцию для получения команд, которые этим приложением зарегистрированы

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual void OnCommand(
	Document pDocument,
	int id
)
```




#### Параметры

pDocument [Document](T_TFlex_Model_Document.md)
    Документ, который является активным в момент выполнения данной команды
id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды, под которым приложение эту команду зарегестрировало

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[OnCommand - перегрузка](Overload_TFlex_Plugin_OnCommand.md)

[TFlex - пространство имён](N_TFlex.md)