

Руководство по T-FLEX CAD Open API

# PluginRegisterCommand(Int32, CommandParameters) - метод  
    
Регистрации команды приложения

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected void RegisterCommand(
	int id,
	CommandParameters parameters
)
```




#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды. Он должен быть уникальным в пределах приложения и не требует проверки на несовпадение с командами других приложения и самого T-FLEX CAD
parameters [CommandParameters](T_TFlex_Command_CommandParameters.md)
    Параметры команды

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[RegisterCommand - перегрузка](Overload_TFlex_Plugin_RegisterCommand.md)

[TFlex - пространство имён](N_TFlex.md)