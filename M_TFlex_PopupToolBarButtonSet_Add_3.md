

Руководство по T-FLEX CAD Open API

# PopupToolBarButtonSetAdd(Int32, Plugin) - метод  
  
---  
  
Добавляет в этот набор кнопку вызова указанной команды

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool Add(
	int commandId,
	Plugin plugin
)
```
```vb
Public Function Add ( 
	commandId As Integer,
	plugin As Plugin
) As Boolean
```
```cpp
public:
bool Add(
	int commandId, 
	Plugin^ plugin
)
```


#### Параметры

commandId [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды приложения
plugin [Plugin](T_TFlex_Plugin.md)
    Объект приложения

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)true, если кнопка была добавлена в этот набор; false, если указанный идентификатор команды недействителен или используется одной из кнопок, уже имеющихся в этом наборе

#### Ссылки

[PopupToolBarButtonSet - ](T_TFlex_PopupToolBarButtonSet.md)

[Add - перегрузка](Overload_TFlex_PopupToolBarButtonSet_Add.md)

[TFlex - пространство имён](N_TFlex.md)