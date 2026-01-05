

Руководство по T-FLEX CAD Open API

# BaseControlLostFocus - событие  
  
---  
  
Событие потери фокуса ввода

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<BaseEventArgs> LostFocus
```
```vb
Public Event LostFocus As EventHandler(Of BaseEventArgs)
```
```cpp
public:
 event EventHandler<BaseEventArgs^>^ LostFocus {
	void add (EventHandler<BaseEventArgs^>^ value);
	void remove (EventHandler<BaseEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[BaseEventArgs](T_TFlex_Dialogs_BaseEventArgs.md)

#### Ссылки

[BaseControl - ](T_TFlex_Dialogs_BaseControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)