

Руководство по T-FLEX CAD Open API

# SliderControlValueChanged - событие  
    
Событие смены текущего значения

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<SliderControlValueChangedEventArgs> ValueChanged
```
```vb
Public Event ValueChanged As EventHandler(Of SliderControlValueChangedEventArgs)
```
```cpp
public:
 event EventHandler<SliderControlValueChangedEventArgs^>^ ValueChanged {
	void add (EventHandler<SliderControlValueChangedEventArgs^>^ value);
	void remove (EventHandler<SliderControlValueChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[SliderControlValueChangedEventArgs](T_TFlex_Dialogs_SliderControlValueChangedEventArgs.md)

#### Ссылки

[SliderControl - ](T_TFlex_Dialogs_SliderControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)