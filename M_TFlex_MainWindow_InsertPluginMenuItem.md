

Руководство по T-FLEX CAD Open API

# MainWindowInsertPluginMenuItem - метод  
  
---  
  
Вставить пункт меню приложения

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertPluginMenuItem(
	int command,
	string caption,
	MainWindowInsertMenuPosition position,
	Plugin plugin
)
```
```vb
Public Sub InsertPluginMenuItem ( 
	command As Integer,
	caption As String,
	position As MainWindowInsertMenuPosition,
	plugin As Plugin
)
```
```cpp
public:
void InsertPluginMenuItem(
	int command, 
	String^ caption, 
	MainWindowInsertMenuPosition position, 
	Plugin^ plugin
)
```


#### Параметры

command [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор зарегестрированной в приложении команды
caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Текст пункта меню
position [MainWindowInsertMenuPosition](T_TFlex_MainWindow_InsertMenuPosition.md)
    Место для вставки
plugin [Plugin](T_TFlex_Plugin.md)
    Объект приложения

#### Ссылки

[MainWindow - ](T_TFlex_MainWindow.md)

[TFlex - пространство имён](N_TFlex.md)