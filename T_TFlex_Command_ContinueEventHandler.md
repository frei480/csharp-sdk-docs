

Руководство по T-FLEX CAD Open API

# ContinueEventHandler - делегат  
  
---  
  
Делегат представляющий метод, который будет обрабатывать событие завершения выполнения вложенной команды

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public delegate void ContinueEventHandler(
	Object sender,
	ContinueEventArgs e
)
```
```vb
Public Delegate Sub ContinueEventHandler ( 
	sender As Object,
	e As ContinueEventArgs
)
```
```cpp
public delegate void ContinueEventHandler(
	Object^ sender, 
	ContinueEventArgs^ e
)
```


#### Параметры

sender [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Источник события
e [ContinueEventArgs](T_TFlex_Command_ContinueEventArgs.md)
    Аргументы события

#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)