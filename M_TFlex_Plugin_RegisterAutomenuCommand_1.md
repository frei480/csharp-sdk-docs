

Руководство по T-FLEX CAD Open API

# PluginRegisterAutomenuCommand(Int32, String, Icon) - метод  
  
---  
  
Регистрация команды автоменю

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected void RegisterAutomenuCommand(
	int id,
	string hint,
	Icon icon
)
```
```vb
Protected Sub RegisterAutomenuCommand ( 
	id As Integer,
	hint As String,
	icon As Icon
)
```
```cpp
protected:
void RegisterAutomenuCommand(
	int id, 
	String^ hint, 
	Icon^ icon
)
```


#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды автоменю
hint [String](https://learn.microsoft.com/dotnet/api/system.string)
    Комментарии, отображающиеся при наведении курсора на иконку команды автоменю и в статусной строке
icon [Icon](https://learn.microsoft.com/dotnet/api/system.drawing.icon)
    Иконка команды автоменю (16х16 пикселей)

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[RegisterAutomenuCommand - перегрузка](Overload_TFlex_Plugin_RegisterAutomenuCommand.md)

[TFlex - пространство имён](N_TFlex.md)