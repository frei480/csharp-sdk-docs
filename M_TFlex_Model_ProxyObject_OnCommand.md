

Руководство по T-FLEX CAD Open API

# ProxyObjectOnCommand - метод  
  
---  
  
Метод для обработки команд контекстного меню

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual bool OnCommand(
	int commandID,
	View view
)
```
```vb
Protected Overridable Function OnCommand ( 
	commandID As Integer,
	view As View
) As Boolean
```
```cpp
protected:
virtual bool OnCommand(
	int commandID, 
	View^ view
)
```


#### Параметры

commandID [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды объекта
view [View](T_TFlex_Model_View.md)
    Вид документа

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[ProxyObject - ](T_TFlex_Model_ProxyObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)