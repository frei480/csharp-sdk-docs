

Руководство по T-FLEX CAD Open API

# PluginCommandSelect - событие  
    
Событие, возникающее при выборе объекта

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public event SelectEventHandler Select
```
```vb
Public Event Select As SelectEventHandler
```
```cpp
public:
 event SelectEventHandler^ Select {
	void add (SelectEventHandler^ value);
	void remove (SelectEventHandler^ value);
}
```


#### Значение

[SelectEventHandler](T_TFlex_Command_SelectEventHandler.md)

В обработчике этого события надо отбрасывать неподходящие объекты

#### Ссылки

[PluginCommand - ](T_TFlex_Command_PluginCommand.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)