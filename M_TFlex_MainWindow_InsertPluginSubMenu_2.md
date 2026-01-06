

Руководство по T-FLEX CAD Open API

# MainWindowInsertPluginSubMenu(String, Menu, MainWindowInsertMenuPosition, Plugin) - метод  
    
Вставить подменю приложения

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void InsertPluginSubMenu(
	string caption,
	Menu menu,
	MainWindowInsertMenuPosition position,
	Plugin plugin
)
```
```vb
Public Sub InsertPluginSubMenu ( 
	caption As String,
	menu As Menu,
	position As MainWindowInsertMenuPosition,
	plugin As Plugin
)
```
```cpp
public:
void InsertPluginSubMenu(
	String^ caption, 
	Menu^ menu, 
	MainWindowInsertMenuPosition position, 
	Plugin^ plugin
)
```


#### Параметры

caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название подменю
menu [Menu](T_TFlex_Menu.md)
    Объект подменю
position [MainWindowInsertMenuPosition](T_TFlex_MainWindow_InsertMenuPosition.md)
    Место для вставки
plugin [Plugin](T_TFlex_Plugin.md)
    Объект приложения

#### Ссылки

[MainWindow - ](T_TFlex_MainWindow.md)

[InsertPluginSubMenu - перегрузка](Overload_TFlex_MainWindow_InsertPluginSubMenu.md)

[TFlex - пространство имён](N_TFlex.md)