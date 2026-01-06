

Руководство по T-FLEX CAD Open API

# SelectControlItemSelected - событие  
    
Событие выбора данного элемента

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<SelectControlItemChangedEventArgs> Selected
```
```vb
Public Event Selected As EventHandler(Of SelectControlItemChangedEventArgs)
```
```cpp
public:
 event EventHandler<SelectControlItemChangedEventArgs^>^ Selected {
	void add (EventHandler<SelectControlItemChangedEventArgs^>^ value);
	void remove (EventHandler<SelectControlItemChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[SelectControlItemChangedEventArgs](T_TFlex_Dialogs_SelectControlItemChangedEventArgs.md)

#### Ссылки

[SelectControlItem - ](T_TFlex_Dialogs_SelectControlItem.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)