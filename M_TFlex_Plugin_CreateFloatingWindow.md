

Руководство по T-FLEX CAD Open API

# PluginCreateFloatingWindow(UInt32, String) - метод  
  
---  
  
Создать плавающее окно приложения

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected PluginFloatingWindow CreateFloatingWindow(
	uint id,
	string title
)
```
```vb
Protected Function CreateFloatingWindow ( 
	id As UInteger,
	title As String
) As PluginFloatingWindow
```
```cpp
protected:
PluginFloatingWindow^ CreateFloatingWindow(
	unsigned int id, 
	String^ title
)
```


#### Параметры

id [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Идентификатор окна
title [String](https://learn.microsoft.com/dotnet/api/system.string)
    Заголовок окна

#### Возвращаемое значение

[PluginFloatingWindow](T_TFlex_PluginFloatingWindow.md)

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[CreateFloatingWindow - перегрузка](Overload_TFlex_Plugin_CreateFloatingWindow.md)

[TFlex - пространство имён](N_TFlex.md)