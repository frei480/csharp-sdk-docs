

Руководство по T-FLEX CAD Open API

# PickPointMouseMove - делегат  
    
Делегат представляющий метод, который будет обрабатывать событие перемещения мыши при вызове метода PickPoint

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public delegate void PickPointMouseMove(
	Object sender,
	PickPointEventArgs e
)
```
```vb
Public Delegate Sub PickPointMouseMove ( 
	sender As Object,
	e As PickPointEventArgs
)
```
```cpp
public delegate void PickPointMouseMove(
	Object^ sender, 
	PickPointEventArgs^ e
)
```


#### Параметры

sender [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Источник события
e [PickPointEventArgs](T_TFlex_PickPointEventArgs.md)
    Аргументы собятия

#### Ссылки

[TFlex - пространство имён](N_TFlex.md)