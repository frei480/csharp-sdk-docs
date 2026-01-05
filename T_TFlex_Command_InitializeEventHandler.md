

Руководство по T-FLEX CAD Open API

# InitializeEventHandler - делегат  
  
---  
  
Делегат представляющий метод, который будет обрабатывать событие инициализации команды приложения

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public delegate void InitializeEventHandler(
	Object sender,
	InitializeEventArgs e
)
```
```vb
Public Delegate Sub InitializeEventHandler ( 
	sender As Object,
	e As InitializeEventArgs
)
```
```cpp
public delegate void InitializeEventHandler(
	Object^ sender, 
	InitializeEventArgs^ e
)
```


#### Параметры

sender [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Источник события
e [InitializeEventArgs](T_TFlex_Command_InitializeEventArgs.md)
    Аргументы события

#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)