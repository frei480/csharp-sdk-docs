

Руководство по T-FLEX CAD Open API

# PluginCreateToolbar(String, Int32) - метод  
    
Создать панель инструментов

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected void CreateToolbar(
	string Caption,
	int[] CmdIDs
)
```
```vb
Protected Sub CreateToolbar ( 
	Caption As String,
	CmdIDs As Integer()
)
```
```cpp
protected:
void CreateToolbar(
	String^ Caption, 
	array<int>^ CmdIDs
)
```


#### Параметры

Caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название панели
CmdIDs [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Массив идентификаторов команд приложения

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[CreateToolbar - перегрузка](Overload_TFlex_Plugin_CreateToolbar.md)

[TFlex - пространство имён](N_TFlex.md)