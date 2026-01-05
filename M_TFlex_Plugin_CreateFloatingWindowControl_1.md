

Руководство по T-FLEX CAD Open API

# PluginCreateFloatingWindowControl(UInt32, PropertiesWindowFormBase) - метод  
  
---  
**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual bool CreateFloatingWindowControl(
	uint id,
	out PropertiesWindowFormBase control
)
```
```vb
Protected Overridable Function CreateFloatingWindowControl ( 
	id As UInteger,
	<OutAttribute> ByRef control As PropertiesWindowFormBase
) As Boolean
```
```cpp
protected:
virtual bool CreateFloatingWindowControl(
	unsigned int id, 
	[OutAttribute] PropertiesWindowFormBase^% control
)
```


#### Параметры

id [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    
control [PropertiesWindowFormBase](T_TFlex_Command_PropertiesWindowFormBase.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[CreateFloatingWindowControl - перегрузка](Overload_TFlex_Plugin_CreateFloatingWindowControl.md)

[TFlex - пространство имён](N_TFlex.md)