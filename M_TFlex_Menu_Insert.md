

Руководство по T-FLEX CAD Open API

# MenuInsert - метод  
    
Вставить пункт меню

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int index,
	int command,
	string caption,
	Plugin plugin
)
```
```vb
Public Sub Insert ( 
	index As Integer,
	command As Integer,
	caption As String,
	plugin As Plugin
)
```
```cpp
public:
void Insert(
	int index, 
	int command, 
	String^ caption, 
	Plugin^ plugin
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер пункта меню 
command [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор зарегестрированной в приложении команды
caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название пунтка меню
plugin [Plugin](T_TFlex_Plugin.md)
    Объект приложения

#### Ссылки

[Menu - ](T_TFlex_Menu.md)

[TFlex - пространство имён](N_TFlex.md)