

Руководство по T-FLEX CAD Open API

# PluginCommandContinue - событие  
  
---  
  
Событие завершения выполнения вложенной команды

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public event ContinueEventHandler Continue
```
```vb
Public Event Continue As ContinueEventHandler
```
```cpp
public:
 event ContinueEventHandler^ Continue {
	void add (ContinueEventHandler^ value);
	void remove (ContinueEventHandler^ value);
}
```


#### Значение

[ContinueEventHandler](T_TFlex_Command_ContinueEventHandler.md)

Данное событие необходимо реализовать для того, чтобы получить управление при завершении вложенной команды и код её завершения

#### Ссылки

[PluginCommand - ](T_TFlex_Command_PluginCommand.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)