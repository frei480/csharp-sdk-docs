

Руководство по T-FLEX CAD Open API

# SelectionContainerIsSelected - метод  
  
---  
  
Проверка, является ли объект выбранным

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool IsSelected(
	ModelObject obj
)
```
```vb
Public Function IsSelected ( 
	obj As ModelObject
) As Boolean
```
```cpp
public:
bool IsSelected(
	ModelObject^ obj
)
```


#### Параметры

obj [ModelObject](T_TFlex_Model_ModelObject.md)
    Объект для которого производится проверка

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)True, если данный объект является выбранным, то есть находится в контейнере выбранных объектов

Данная функция выполняет проверку на наличие указанного объекта в контейнере выбранных объектов

#### Ссылки

[SelectionContainer - ](T_TFlex_Model_SelectionContainer.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)