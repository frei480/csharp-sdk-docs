

Руководство по T-FLEX CAD Open API

# PluginCommandShowCursor - событие  
    
Событие, возникающее при прорисовке динамического курсора при перемещении мыши

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public event MouseEventHandler ShowCursor
```
```vb
Public Event ShowCursor As MouseEventHandler
```
```cpp
public:
 event MouseEventHandler^ ShowCursor {
	void add (MouseEventHandler^ value);
	void remove (MouseEventHandler^ value);
}
```


#### Значение

[MouseEventHandler](T_TFlex_Command_MouseEventHandler.md)

Данное событие необходимо реализовать в тот момент, когда требуется прорисовка динамического курсора при перемещении мыши

#### Ссылки

[PluginCommand - ](T_TFlex_Command_PluginCommand.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)