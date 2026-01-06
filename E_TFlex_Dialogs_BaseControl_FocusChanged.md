

Руководство по T-FLEX CAD Open API

# BaseControlFocusChanged - событие  
    
Событие получения либо потери фокуса ввода

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<FocusChangedEventArgs> FocusChanged
```
```vb
Public Event FocusChanged As EventHandler(Of FocusChangedEventArgs)
```
```cpp
public:
 event EventHandler<FocusChangedEventArgs^>^ FocusChanged {
	void add (EventHandler<FocusChangedEventArgs^>^ value);
	void remove (EventHandler<FocusChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[FocusChangedEventArgs](T_TFlex_Dialogs_FocusChangedEventArgs.md)

#### Ссылки

[BaseControl - ](T_TFlex_Dialogs_BaseControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)