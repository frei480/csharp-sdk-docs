

Руководство по T-FLEX CAD Open API

# PluginCreateHelpMenuItem - метод  
    
Создать пункт меню в меню справки

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected void CreateHelpMenuItem(
	string caption,
	int commandId,
	int position
)
```
```vb
Protected Sub CreateHelpMenuItem ( 
	caption As String,
	commandId As Integer,
	position As Integer
)
```
```cpp
protected:
void CreateHelpMenuItem(
	String^ caption, 
	int commandId, 
	int position
)
```


#### Параметры

caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название пункта
commandId [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды
position [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Позиция пункта в меню

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)