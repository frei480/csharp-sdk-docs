

Руководство по T-FLEX CAD Open API

# MessagesBarMessageButtonClicked - свойство  
    
Обработчик события нажатия на кнопки

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public EventHandler<MessagesBarClickEventArgs> ButtonClicked { get; set; }
```
```vb
Public Property ButtonClicked As EventHandler(Of MessagesBarClickEventArgs)
	Get
	Set
```
```cpp
public:
property EventHandler<MessagesBarClickEventArgs^>^ ButtonClicked {
	EventHandler<MessagesBarClickEventArgs^>^ get ();
	void set (EventHandler<MessagesBarClickEventArgs^>^ value);
}
```


#### Значение свойства

[EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[MessagesBarClickEventArgs](T_TFlex_MessagesBarClickEventArgs.md)

#### Ссылки

[MessagesBarMessage - ](T_TFlex_MessagesBarMessage.md)

[TFlex - пространство имён](N_TFlex.md)