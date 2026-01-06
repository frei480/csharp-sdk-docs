

Руководство по T-FLEX CAD Open API

# SelectionContainerSelect(ModelObject, SelectionContainerMarkType) - метод  
    
Выбрать объект

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Select(
	ModelObject obj,
	SelectionContainerMarkType style
)
```




#### Параметры

obj [ModelObject](T_TFlex_Model_ModelObject.md)
    Объект, который требуется выбрать (поместить в контейнер выбранных объектов
style [SelectionContainerMarkType](T_TFlex_Model_SelectionContainer_MarkType.md)
    Стиль маркировки объекта

Данная функция помещает указанный объект в контейнер выбранных объектов. При этом объект помечается на всех видах документа, на которых объект является видимым. Для отмены выбора объекта можно воспользоваться функцией Deselect или DeselectAll

#### Ссылки

[SelectionContainer - ](T_TFlex_Model_SelectionContainer.md)

[Select - перегрузка](Overload_TFlex_Model_SelectionContainer_Select.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)