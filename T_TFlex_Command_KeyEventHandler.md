

Руководство по T-FLEX CAD Open API

# KeyEventHandler - делегат  
  
---  
  
Делегат представляющий метод, который будет обрабатывать событие, возникающее при нажатии клавиши клавиатуры или кнопки автоменю

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public delegate void KeyEventHandler(
	Object sender,
	KeyEventArgs e
)
```
```vb
Public Delegate Sub KeyEventHandler ( 
	sender As Object,
	e As KeyEventArgs
)
```
```cpp
public delegate void KeyEventHandler(
	Object^ sender, 
	KeyEventArgs^ e
)
```


#### Параметры

sender [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Источник события
e [KeyEventArgs](T_TFlex_Command_KeyEventArgs.md)
    Аргументы события

#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)