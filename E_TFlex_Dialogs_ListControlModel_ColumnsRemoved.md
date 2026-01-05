

Руководство по T-FLEX CAD Open API

# ListControlModelColumnsRemoved - событие  
  
---  
  
Событие удаления столбцов

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ListControlModelInsertRemoveEventArgs> ColumnsRemoved
```
```vb
Public Event ColumnsRemoved As EventHandler(Of ListControlModelInsertRemoveEventArgs)
```
```cpp
public:
 event EventHandler<ListControlModelInsertRemoveEventArgs^>^ ColumnsRemoved {
	void add (EventHandler<ListControlModelInsertRemoveEventArgs^>^ value);
	void remove (EventHandler<ListControlModelInsertRemoveEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ListControlModelInsertRemoveEventArgs](T_TFlex_Dialogs_ListControlModelInsertRemoveEventArgs.md)

#### Ссылки

[ListControlModel - ](T_TFlex_Dialogs_ListControlModel.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)