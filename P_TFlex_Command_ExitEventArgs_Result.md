

Руководство по T-FLEX CAD Open API

# ExitEventArgsResult - свойство  
    
Объект, который необходимо передать из вложенной команды в вызывающую

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Object Result { set; }
```
```vb
Public WriteOnly Property Result As Object
	Set
```
```cpp
public:
property Object^ Result {
	void set (Object^ value);
}
```


#### Значение свойства

[Object](https://learn.microsoft.com/dotnet/api/system.object)

Применяется только для вложенных команд приложения. Вложенной командой называется команда, функция TFlex.Command.PluginCommand.Run(TFlex.Model.View, bool) которой вызвана внутри обработчика выполнения другой (вызывающей) команды

#### Ссылки

[ExitEventArgs - ](T_TFlex_Command_ExitEventArgs.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)