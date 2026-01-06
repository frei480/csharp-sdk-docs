

Руководство по T-FLEX CAD Open API

# ObjectSelectControlStateUpdated - событие  
    
Событие изменения состояния

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ObjectSelectControlStateUpdateEventArgs> StateUpdated
```
```vb
Public Event StateUpdated As EventHandler(Of ObjectSelectControlStateUpdateEventArgs)
```
```cpp
public:
 event EventHandler<ObjectSelectControlStateUpdateEventArgs^>^ StateUpdated {
	void add (EventHandler<ObjectSelectControlStateUpdateEventArgs^>^ value);
	void remove (EventHandler<ObjectSelectControlStateUpdateEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ObjectSelectControlStateUpdateEventArgs](T_TFlex_Dialogs_ObjectSelectControlStateUpdateEventArgs.md)

#### Ссылки

[ObjectSelectControl - ](T_TFlex_Dialogs_ObjectSelectControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)