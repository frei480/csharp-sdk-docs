

Руководство по T-FLEX CAD Open API

# NumericInputControlValueChanged - событие  
  
---  
  
Событие изменения значения

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ValueChangedEventArgs> ValueChanged
```
```vb
Public Event ValueChanged As EventHandler(Of ValueChangedEventArgs)
```
```cpp
public:
 event EventHandler<ValueChangedEventArgs^>^ ValueChanged {
	void add (EventHandler<ValueChangedEventArgs^>^ value);
	void remove (EventHandler<ValueChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ValueChangedEventArgs](T_TFlex_Dialogs_ValueChangedEventArgs.md)

#### Ссылки

[NumericInputControl - ](T_TFlex_Dialogs_NumericInputControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)