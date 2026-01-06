

Руководство по T-FLEX CAD Open API

# PopupToolBarButtonSetContains(Int32, Plugin) - метод  
    
Определяет, есть в этом наборе указанная кнопка или нет

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool Contains(
	int commandId,
	Plugin plugin
)
```




#### Параметры

commandId [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды приложения
plugin [Plugin](T_TFlex_Plugin.md)
    Объект приложения

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)true, если этот набор содержит кнопку вызова указанной команды, иначе false

#### Ссылки

[PopupToolBarButtonSet - ](T_TFlex_PopupToolBarButtonSet.md)

[Contains - перегрузка](Overload_TFlex_PopupToolBarButtonSet_Contains.md)

[TFlex - пространство имён](N_TFlex.md)