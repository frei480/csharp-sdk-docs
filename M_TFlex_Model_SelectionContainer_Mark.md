

Руководство по T-FLEX CAD Open API

# SelectionContainerMark - метод  
  
---  
  
Маркировать объект

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Mark(
	ModelObject obj,
	SelectionContainerMarkType style
)
```
```vb
Public Sub Mark ( 
	obj As ModelObject,
	style As SelectionContainerMarkType
)
```
```cpp
public:
void Mark(
	ModelObject^ obj, 
	SelectionContainerMarkType style
)
```


#### Параметры

obj [ModelObject](T_TFlex_Model_ModelObject.md)
    Объект, который требуется маркировать
style [SelectionContainerMarkType](T_TFlex_Model_SelectionContainer_MarkType.md)
    Стиль маркировки

Данная функция помещает указанный объект в контейнер маркированных объектов. Для отмены маркирования объекта можно воспользоваться функцией Unmark

#### Ссылки

[SelectionContainer - ](T_TFlex_Model_SelectionContainer.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)