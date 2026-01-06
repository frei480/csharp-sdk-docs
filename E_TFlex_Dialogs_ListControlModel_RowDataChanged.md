

Руководство по T-FLEX CAD Open API

# ListControlModelRowDataChanged - событие  
    
Событие изменения данных строки списка

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ListControlModelRowDataChangedEventArgs> RowDataChanged
```
```vb
Public Event RowDataChanged As EventHandler(Of ListControlModelRowDataChangedEventArgs)
```
```cpp
public:
 event EventHandler<ListControlModelRowDataChangedEventArgs^>^ RowDataChanged {
	void add (EventHandler<ListControlModelRowDataChangedEventArgs^>^ value);
	void remove (EventHandler<ListControlModelRowDataChangedEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ListControlModelRowDataChangedEventArgs](T_TFlex_Dialogs_ListControlModelRowDataChangedEventArgs.md)

#### Ссылки

[ListControlModel - ](T_TFlex_Dialogs_ListControlModel.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)