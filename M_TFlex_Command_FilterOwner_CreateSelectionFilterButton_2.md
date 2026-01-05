

Руководство по T-FLEX CAD Open API

# FilterOwnerCreateSelectionFilterButton(Guid, String, ObjectType) - метод  
  
---  
  
Создать кнопку селекции

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected SelectionFilterButton CreateSelectionFilterButton(
	Guid iconId,
	string toolTip,
	ObjectType neighbor
)
```
```vb
Protected Function CreateSelectionFilterButton ( 
	iconId As Guid,
	toolTip As String,
	neighbor As ObjectType
) As SelectionFilterButton
```
```cpp
protected:
SelectionFilterButton^ CreateSelectionFilterButton(
	Guid iconId, 
	String^ toolTip, 
	ObjectType neighbor
)
```


#### Параметры

iconId [Guid](https://learn.microsoft.com/dotnet/api/system.guid)
    Идентификатор, использованный для регистрации иконки при помощи [!:TFlex::Command::CustomCommand::RegisterAutomenuIcon]
toolTip [String](https://learn.microsoft.com/dotnet/api/system.string)
    Подсказка для кнопки
neighbor [ObjectType](T_TFlex_Model_ObjectType.md)
    Тип модельного объекта, соответствующий существующей кнопке селекции, которая должна предшествовать новой

#### Возвращаемое значение

[SelectionFilterButton](T_TFlex_Command_SelectionFilterButton.md)Созданная кнопка либо null в случае ошибки

Добавляет кнопку в конец панели, если neighbor не соответствует ни одной из существующих кнопок

#### Ссылки

[FilterOwner - ](T_TFlex_Command_FilterOwner.md)

[CreateSelectionFilterButton - перегрузка](Overload_TFlex_Command_FilterOwner_CreateSelectionFilterButton.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)