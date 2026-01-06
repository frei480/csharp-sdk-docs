

Руководство по T-FLEX CAD Open API

# PluginCommandOnShowCursor - метод  
    
Динамическая отрисовка курсора

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual void OnShowCursor(
	MouseEventArgs e
)
```
```vb
Public Overridable Sub OnShowCursor ( 
	e As MouseEventArgs
)
```
```cpp
public:
virtual void OnShowCursor(
	MouseEventArgs^ e
)
```


#### Параметры

e [MouseEventArgs](T_TFlex_Command_MouseEventArgs.md)
    Аргументы события

Данная функция вызывается в тот момент, когда требуется прорисовка динамического курсора при перемещении мыши

#### Ссылки

[PluginCommand - ](T_TFlex_Command_PluginCommand.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)