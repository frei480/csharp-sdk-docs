

Руководство по T-FLEX CAD Open API

# SelectControlSelectedItemChanged - событие  
  
---  
  
Событие смены выбранного элемента

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<SelectControlItemChangedEventArgs> SelectedItemChanged
```
```vb
Public Event SelectedItemChanged As EventHandler(Of SelectControlItemChangedEventArgs)
```
```cpp
public:
 event EventHandler<SelectControlItemChangedEventArgs^>^ SelectedItemChanged {
	void add (EventHandler<SelectControlItemChangedEventArgs^>^ value);
	void remove (EventHandler<SelectControlItemChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[SelectControlItemChangedEventArgs](T_TFlex_Dialogs_SelectControlItemChangedEventArgs.md)

#### Ссылки

[SelectControl - ](T_TFlex_Dialogs_SelectControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)