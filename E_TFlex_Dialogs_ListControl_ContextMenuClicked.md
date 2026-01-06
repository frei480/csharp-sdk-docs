

Руководство по T-FLEX CAD Open API

# ListControlContextMenuClicked - событие  
    
Событие о нажатии в контекстном меню

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ListControlContextMenuClickedEventArgs> ContextMenuClicked
```
```vb
Public Event ContextMenuClicked As EventHandler(Of ListControlContextMenuClickedEventArgs)
```
```cpp
public:
 event EventHandler<ListControlContextMenuClickedEventArgs^>^ ContextMenuClicked {
	void add (EventHandler<ListControlContextMenuClickedEventArgs^>^ value);
	void remove (EventHandler<ListControlContextMenuClickedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ListControlContextMenuClickedEventArgs](T_TFlex_Dialogs_ListControlContextMenuClickedEventArgs.md)

#### Ссылки

[ListControl - ](T_TFlex_Dialogs_ListControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)