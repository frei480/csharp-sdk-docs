

Руководство по T-FLEX CAD Open API

# MessagesBarAddMessage(String, String, Document) - метод  
  
---  
  
Добавить сообщение

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public IntPtr AddMessage(
	string title,
	string text,
	Document document
)
```
```vb
Public Function AddMessage ( 
	title As String,
	text As String,
	document As Document
) As IntPtr
```
```cpp
public:
IntPtr AddMessage(
	String^ title, 
	String^ text, 
	Document^ document
)
```


#### Параметры

title [String](https://learn.microsoft.com/dotnet/api/system.string)
    Заголовок
text [String](https://learn.microsoft.com/dotnet/api/system.string)
    Сообщение
document [Document](T_TFlex_Model_Document.md)
    Связанный документ

#### Возвращаемое значение

[IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)

#### Ссылки

[MessagesBar - ](T_TFlex_MessagesBar.md)

[AddMessage - перегрузка](Overload_TFlex_MessagesBar_AddMessage.md)

[TFlex - пространство имён](N_TFlex.md)