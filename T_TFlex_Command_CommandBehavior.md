

Руководство по T-FLEX CAD Open API

# CommandBehavior - перечисление  
    
Поведение команды

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
[FlagsAttribute]
public enum CommandBehavior
```
```vb
<FlagsAttribute>
Public Enumeration CommandBehavior
```
```cpp
[FlagsAttribute]
public enum class CommandBehavior
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Default | 0 |  |
| MouseButtonsUpEvents | 1 | Command expects events to fire when mouse buttons come up |
| MouseButtonsPressedIn2dView | 2 | Key pressed event for mouse buttons will fire for 2D view |
| DisableAutomenuIn3DView | 4 | Automenu commands will be disabled when 3d view is active |
| StoreStatesForRollback | 8 | Flag for CustomCommand. If it's on CustomCommand.GoToPrevState call will activate previous state otherwise it will terminate command. |
  
#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)