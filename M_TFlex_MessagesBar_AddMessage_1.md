

Руководство по T-FLEX CAD Open API

# MessagesBarAddMessage(String, String, Document, ListMessagesBarButton, EventHandlerMessagesBarClickEventArgs, IntPtr) - метод  
  **Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public IntPtr AddMessage(
	string title,
	string text,
	Document document,
	List<MessagesBarButton> buttons,
	EventHandler<MessagesBarClickEventArgs> buttonClicked,
	IntPtr tag
)
```




#### Параметры

title [String](https://learn.microsoft.com/dotnet/api/system.string)
    
text [String](https://learn.microsoft.com/dotnet/api/system.string)
    
document [Document](T_TFlex_Model_Document.md)
    
buttons [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[MessagesBarButton](T_TFlex_MessagesBarButton.md)
    
buttonClicked [EventHandler](https://learn.microsoft.com/dotnet/api/system.eventhandler-1)[MessagesBarClickEventArgs](T_TFlex_MessagesBarClickEventArgs.md)
    
tag [IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)
    

#### Возвращаемое значение

[IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)

#### Ссылки

[MessagesBar - ](T_TFlex_MessagesBar.md)

[AddMessage - перегрузка](Overload_TFlex_MessagesBar_AddMessage.md)

[TFlex - пространство имён](N_TFlex.md)