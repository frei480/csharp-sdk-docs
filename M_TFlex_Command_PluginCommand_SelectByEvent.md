

Руководство по T-FLEX CAD Open API

# PluginCommandSelectByEvent - метод  
  
---  
  
Функция выбора объекта

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected ModelObject SelectByEvent(
	CursorEventArgs ev,
	bool mark
)
```
```vb
Protected Function SelectByEvent ( 
	ev As CursorEventArgs,
	mark As Boolean
) As ModelObject
```
```cpp
protected:
ModelObject^ SelectByEvent(
	CursorEventArgs^ ev, 
	bool mark
)
```


#### Параметры

ev [CursorEventArgs](T_TFlex_Command_CursorEventArgs.md)
    Аргументы события, возникающие при манипуляциях с курсором
mark [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Подсвечивать выбираемые объекты

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)

Этим методом можно пользоваться в обработчике щелчка мыши или нажатия на Enter. Изнутри метода вызывается обработчик Select, выбранный объект помещается в контейнер (см. [SelectionContainer](T_TFlex_Model_SelectionContainer.md)).

#### Ссылки

[PluginCommand - ](T_TFlex_Command_PluginCommand.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)