

Руководство по T-FLEX CAD Open API

# BaseControlActiveChanged - событие  
    
Событие активации либо деактивации элемента

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ActiveChangedEventArgs> ActiveChanged
```
```vb
Public Event ActiveChanged As EventHandler(Of ActiveChangedEventArgs)
```
```cpp
public:
 event EventHandler<ActiveChangedEventArgs^>^ ActiveChanged {
	void add (EventHandler<ActiveChangedEventArgs^>^ value);
	void remove (EventHandler<ActiveChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ActiveChangedEventArgs](T_TFlex_Dialogs_ActiveChangedEventArgs.md)

#### Ссылки

[BaseControl - ](T_TFlex_Dialogs_BaseControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)