

Руководство по T-FLEX CAD Open API

# ListControlItemHighlighted - событие  
  
---  
  
Событие наведения указателя мыши на объект в списке

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ListControlHighlightEventArgs> ItemHighlighted
```
```vb
Public Event ItemHighlighted As EventHandler(Of ListControlHighlightEventArgs)
```
```cpp
public:
 event EventHandler<ListControlHighlightEventArgs^>^ ItemHighlighted {
	void add (EventHandler<ListControlHighlightEventArgs^>^ value);
	void remove (EventHandler<ListControlHighlightEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ListControlHighlightEventArgs](T_TFlex_Dialogs_ListControlHighlightEventArgs.md)

#### Ссылки

[ListControl - ](T_TFlex_Dialogs_ListControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)