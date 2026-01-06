

Руководство по T-FLEX CAD Open API

# MainWindowInsertPluginSubMenu(String, MainWindowInsertMenuPosition, Plugin) - метод  
    
**Примечание: Данный API устарел.**

Вставить подменю приложения

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("Use method "void InsertPluginSubMenu(String caption, TFlex::Menu menu, InsertMenuPosition position, Plugin plugin)"")]
public Menu InsertPluginSubMenu(
	string caption,
	MainWindowInsertMenuPosition position,
	Plugin plugin
)
```
```vb
<ObsoleteAttribute("Use method "void InsertPluginSubMenu(String caption, TFlex::Menu menu, InsertMenuPosition position, Plugin plugin)"")>
Public Function InsertPluginSubMenu ( 
	caption As String,
	position As MainWindowInsertMenuPosition,
	plugin As Plugin
) As Menu
```
```cpp
public:
[ObsoleteAttribute(L"Use method "void InsertPluginSubMenu(String caption, TFlex::Menu menu, InsertMenuPosition position, Plugin plugin)"")]
Menu^ InsertPluginSubMenu(
	String^ caption, 
	MainWindowInsertMenuPosition position, 
	Plugin^ plugin
)
```


#### Параметры

caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название подменю
position [MainWindowInsertMenuPosition](T_TFlex_MainWindow_InsertMenuPosition.md)
    Место для вставки
plugin [Plugin](T_TFlex_Plugin.md)
    Объект приложения

#### Возвращаемое значение

[Menu](T_TFlex_Menu.md)

#### Ссылки

[MainWindow - ](T_TFlex_MainWindow.md)

[InsertPluginSubMenu - перегрузка](Overload_TFlex_MainWindow_InsertPluginSubMenu.md)

[TFlex - пространство имён](N_TFlex.md)