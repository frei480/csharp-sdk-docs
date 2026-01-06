

Руководство по T-FLEX CAD Open API

# MenuAppend(Int32, String, Boolean, Boolean, Plugin) - метод  
    
Добавить пункт меню

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Append(
	int command,
	string caption,
	bool enable,
	bool check,
	Plugin plugin
)
```




#### Параметры

command [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор зарегестрированной в приложении команды
caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название пунтка меню
enable [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Доступность пункта меню
check [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Устанавливает галочку напротив пункта меню
plugin [Plugin](T_TFlex_Plugin.md)
    Объект приложения

#### Ссылки

[Menu - ](T_TFlex_Menu.md)

[Append - перегрузка](Overload_TFlex_Menu_Append.md)

[TFlex - пространство имён](N_TFlex.md)