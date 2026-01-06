

Руководство по T-FLEX CAD Open API

# ObjectSelectControlObjectReplacedByUser - событие  
    
Событие замены объекта пользователем

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public event EventHandler<ObjectSelectControlReplaceObjectEventArgs> ObjectReplacedByUser
```
```vb
Public Event ObjectReplacedByUser As EventHandler(Of ObjectSelectControlReplaceObjectEventArgs)
```
```cpp
public:
 event EventHandler<ObjectSelectControlReplaceObjectEventArgs^>^ ObjectReplacedByUser {
	void add (EventHandler<ObjectSelectControlReplaceObjectEventArgs^>^ value);
	void remove (EventHandler<ObjectSelectControlReplaceObjectEventArgs^>^ value);
}
```


#### Значение

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[ObjectSelectControlReplaceObjectEventArgs](T_TFlex_Dialogs_ObjectSelectControlReplaceObjectEventArgs.md)

#### Ссылки

[ObjectSelectControl - ](T_TFlex_Dialogs_ObjectSelectControl.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)