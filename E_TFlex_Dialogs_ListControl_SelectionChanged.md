

Руководство по T-FLEX CAD Open API

# ListControlSelectionChanged - событие  
    
Событие о смене выбранных элементов списка

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ListControlSelectionChangedEventArgs> SelectionChanged
```
```vb
Public Event SelectionChanged As EventHandler(Of ListControlSelectionChangedEventArgs)
```
```cpp
public:
 event EventHandler<ListControlSelectionChangedEventArgs^>^ SelectionChanged {
	void add (EventHandler<ListControlSelectionChangedEventArgs^>^ value);
	void remove (EventHandler<ListControlSelectionChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ListControlSelectionChangedEventArgs](T_TFlex_Dialogs_ListControlSelectionChangedEventArgs.md)

#### Ссылки

[ListControl - ](T_TFlex_Dialogs_ListControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)