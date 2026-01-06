

Руководство по T-FLEX CAD Open API

# PluginCommandExit - событие  
    
Событие завершения выполнения команды

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public event ExitEventHandler Exit
```
```vb
Public Event Exit As ExitEventHandler
```
```cpp
public:
 event ExitEventHandler^ Exit {
	void add (ExitEventHandler^ value);
	void remove (ExitEventHandler^ value);
}
```


#### Значение

[ExitEventHandler](T_TFlex_Command_ExitEventHandler.md)

Данное событие необходимо реализовать для того, чтобы получить управление в момент завершения выполнения команды. Это сообщение приходит последним в процессе выполнения команды

#### Ссылки

[PluginCommand - ](T_TFlex_Command_PluginCommand.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)