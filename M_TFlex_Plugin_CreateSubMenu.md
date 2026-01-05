

Руководство по T-FLEX CAD Open API

# PluginCreateSubMenu - метод  
  
---  
  
Создать подменю в меню приложения

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected void CreateSubMenu(
	Menu menu,
	string caption,
	int position
)
```
```vb
Protected Sub CreateSubMenu ( 
	menu As Menu,
	caption As String,
	position As Integer
)
```
```cpp
protected:
void CreateSubMenu(
	Menu^ menu, 
	String^ caption, 
	int position
)
```


#### Параметры

menu [Menu](T_TFlex_Menu.md)
    Меню для добавления
caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название панели
position [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Позиция подменю в системном меню

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)