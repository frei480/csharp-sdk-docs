

Руководство по T-FLEX CAD Open API

# SimpleListControlCheckStateChanged - событие  
  
---  
  
Событие смены значения чекбокса

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<SimpleListControlCheckStateChangedEventArgs> CheckStateChanged
```
```vb
Public Event CheckStateChanged As EventHandler(Of SimpleListControlCheckStateChangedEventArgs)
```
```cpp
public:
 event EventHandler<SimpleListControlCheckStateChangedEventArgs^>^ CheckStateChanged {
	void add (EventHandler<SimpleListControlCheckStateChangedEventArgs^>^ value);
	void remove (EventHandler<SimpleListControlCheckStateChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[SimpleListControlCheckStateChangedEventArgs](T_TFlex_Dialogs_SimpleListControlCheckStateChangedEventArgs.md)

#### Ссылки

[SimpleListControl - ](T_TFlex_Dialogs_SimpleListControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)