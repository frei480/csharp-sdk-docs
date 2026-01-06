

Руководство по T-FLEX CAD Open API

# PluginCommandOnExit - метод  
    
Обработчик выхода из команды

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual void OnExit(
	ExitEventArgs e
)
```
```vb
Public Overridable Sub OnExit ( 
	e As ExitEventArgs
)
```
```cpp
public:
virtual void OnExit(
	ExitEventArgs^ e
)
```


#### Параметры

e [ExitEventArgs](T_TFlex_Command_ExitEventArgs.md)
    Аргументы события

Данную функцию необходимо переопределить для того, чтобы получить управление в момент завершения выполнения команды. Это сообщение приходит последним в процессе выполнения команды

#### Ссылки

[PluginCommand - ](T_TFlex_Command_PluginCommand.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)