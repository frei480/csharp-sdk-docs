

Руководство по T-FLEX CAD Open API

# ControlRMouseDown - делегат  
  
---  
  
Делегат представляющий метод, который будет обрабатывать событие, происходящеe при нажатии правой кнопки мыши, если указатель мыши находится на визуальном элементе управления.

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public delegate void ControlRMouseDown(
	Object sender,
	ControlEventArgs e
)
```
```vb
Public Delegate Sub ControlRMouseDown ( 
	sender As Object,
	e As ControlEventArgs
)
```
```cpp
public delegate void ControlRMouseDown(
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