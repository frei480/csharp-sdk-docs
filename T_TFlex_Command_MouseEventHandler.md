

Руководство по T-FLEX CAD Open API

# MouseEventHandler - делегат  
    
Делегат представляющий метод, который будет обрабатывать событие, возникающее при перемещении курсора

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public delegate void MouseEventHandler(
	Object sender,
	MouseEventArgs e
)
```
```vb
Public Delegate Sub MouseEventHandler ( 
	sender As Object,
	e As MouseEventArgs
)
```
```cpp
public delegate void MouseEventHandler(
	Object^ sender, 
	MouseEventArgs^ e
)
```


#### Параметры

sender [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Источник события
e [MouseEventArgs](T_TFlex_Command_MouseEventArgs.md)
    Аргументы события

#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)