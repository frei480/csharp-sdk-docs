

Руководство по T-FLEX CAD Open API

# SelectionContainerUnmark - метод  
  
---  
  
Отменить маркирования объекта

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Unmark(
	ModelObject obj
)
```
```vb
Public Sub Unmark ( 
	obj As ModelObject
)
```
```cpp
public:
void Unmark(
	ModelObject^ obj
)
```


#### Параметры

obj [ModelObject](T_TFlex_Model_ModelObject.md)
    Объект, выбор которого требуется отменить (удалить из контейнера выбранных объектов.

Данная функция удаляет указанный объект из контейнера маркированных объектов.

#### Ссылки

[SelectionContainer - ](T_TFlex_Model_SelectionContainer.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)