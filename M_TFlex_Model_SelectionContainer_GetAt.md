

Руководство по T-FLEX CAD Open API

# SelectionContainerGetAt - метод  
  
---  
  
Получить выбранный объект по индексу

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ModelObject GetAt(
	int i
)
```
```vb
Public Function GetAt ( 
	i As Integer
) As ModelObject
```
```cpp
public:
ModelObject^ GetAt(
	int i
)
```


#### Параметры

i [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)Объект, находящийся в контейнере выбранных объектов с указанным индексом. 0 в случае ошибки

#### Ссылки

[SelectionContainer - ](T_TFlex_Model_SelectionContainer.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)