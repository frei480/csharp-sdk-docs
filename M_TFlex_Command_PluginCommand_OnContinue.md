

Руководство по T-FLEX CAD Open API

# PluginCommandOnContinue - метод  
    
Обработчик завершения выполнения вложенной команды

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual void OnContinue(
	ContinueEventArgs e
)
```
```vb
Public Overridable Sub OnContinue ( 
	e As ContinueEventArgs
)
```
```cpp
public:
virtual void OnContinue(
	ContinueEventArgs^ e
)
```


#### Параметры

e [ContinueEventArgs](T_TFlex_Command_ContinueEventArgs.md)
    Аргументы события

Данную функцию необходимо переопределить для того, чтобы получить управление при завершении вложенной команды и код её завершения

#### Ссылки

[PluginCommand - ](T_TFlex_Command_PluginCommand.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)