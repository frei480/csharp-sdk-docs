

Руководство по T-FLEX CAD Open API

# PluginRegisterObjectCommand(Int32, String, Icon, Icon) - метод  
    
Регистрация команды объекта

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected void RegisterObjectCommand(
	int id,
	string prompt,
	Icon smallIcon,
	Icon largeIcon
)
```




#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды объекта. Он должен быть уникальным в пределах приложения и не требует проверки на несовпадение с командами других приложения и самого T-FLEX CAD
prompt [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название команды объекта
smallIcon [Icon](https://learn.microsoft.com/dotnet/api/system.drawing.icon)
    Маленькая иконка команды (16х16 пикселей)
largeIcon [Icon](https://learn.microsoft.com/dotnet/api/system.drawing.icon)
    Большая иконка команды (24х24 пикселя)

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[RegisterObjectCommand - перегрузка](Overload_TFlex_Plugin_RegisterObjectCommand.md)

[TFlex - пространство имён](N_TFlex.md)