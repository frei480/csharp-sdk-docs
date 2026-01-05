

Руководство по T-FLEX CAD Open API

# SelectionContainerDeselect - метод  
  
---  
  
Отменить выбор объекта

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Deselect(
	ModelObject obj
)
```
```vb
Public Sub Deselect ( 
	obj As ModelObject
)
```
```cpp
public:
void Deselect(
	ModelObject^ obj
)
```


#### Параметры

obj [ModelObject](T_TFlex_Model_ModelObject.md)
    Объект, выбор которого требуется отменить (удалить из контейнера выбранных объектов.

Данная функция удаляет указанный объект из контейнера выбранных объектов. При этом отменяется пометка этого объекта на всех видах документа, на которых он является видимым.

#### Ссылки

[SelectionContainer - ](T_TFlex_Model_SelectionContainer.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)