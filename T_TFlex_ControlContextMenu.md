

Руководство по T-FLEX CAD Open API

# ControlContextMenu - делегат  
    
Делегат представляющий метод, который будет обрабатывать событие, происходящее при вызове контекстного меню на визуальном элементе управления

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public delegate void ControlContextMenu(
	Object sender,
	ControlEventArgs e
)
```
```vb
Public Delegate Sub ControlContextMenu ( 
	sender As Object,
	e As ControlEventArgs
)
```
```cpp
public delegate void ControlContextMenu(
	Object^ sender, 
	ControlEventArgs^ e
)
```


#### Параметры

sender [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Источник события
e [ControlEventArgs](T_TFlex_ControlEventArgs.md)
    Аргументы события

#### Ссылки

[TFlex - пространство имён](N_TFlex.md)