

Руководство по T-FLEX CAD Open API

# FilterOwnerCreateSelectionFilterButton(Guid, String, SelectionFilterButton) - метод  
    
Создать кнопку селекции

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected SelectionFilterButton CreateSelectionFilterButton(
	Guid iconId,
	string toolTip,
	SelectionFilterButton neighbor
)
```




#### Параметры

iconId [Guid](https://learn.microsoft.com/dotnet/api/system.guid)
    Идентификатор, использованный для регистрации иконки при помощи [!:TFlex::Command::CustomCommand::RegisterAutomenuIcon]
toolTip [String](https://learn.microsoft.com/dotnet/api/system.string)
    Подсказка для кнопки
neighbor [SelectionFilterButton](T_TFlex_Command_SelectionFilterButton.md)
    Существующая кнопка селекции, которая должна предшествовать новой

#### Возвращаемое значение

[SelectionFilterButton](T_TFlex_Command_SelectionFilterButton.md)Созданная кнопка либо null в случае ошибки

Добавляет кнопку в конец панели, если neighbor не является существующей кнопкой селекции

#### Ссылки

[FilterOwner - ](T_TFlex_Command_FilterOwner.md)

[CreateSelectionFilterButton - перегрузка](Overload_TFlex_Command_FilterOwner_CreateSelectionFilterButton.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)