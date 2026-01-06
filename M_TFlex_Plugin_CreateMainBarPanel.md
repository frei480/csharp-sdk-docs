

Руководство по T-FLEX CAD Open API

# PluginCreateMainBarPanel - метод  
    
Создать панель инструментов

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected void CreateMainBarPanel(
	string caption,
	int[] cmdIDs,
	Guid panelGuid,
	bool showDefaultSet
)
```




#### Параметры

caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название панели
cmdIDs [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Массив идентификаторов команд приложения
panelGuid [Guid](https://learn.microsoft.com/dotnet/api/system.guid)
    GUID панели, которую необходимо присоединить к MainBar-у
showDefaultSet [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    флаг, который отвечает за показ/скрытие набора иконок основных команд

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)