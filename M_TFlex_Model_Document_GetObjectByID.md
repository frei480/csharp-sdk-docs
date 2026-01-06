

Руководство по T-FLEX CAD Open API

# DocumentGetObjectById - метод  
    
Получение объекта по идентификатору

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ModelObject GetObjectById(
	ObjectId id
)
```
```vb
Public Function GetObjectById ( 
	id As ObjectId
) As ModelObject
```
```cpp
public:
ModelObject^ GetObjectById(
	ObjectId^ id
)
```


#### Параметры

id [ObjectId](T_TFlex_Model_ObjectId.md)
    Идентификатор объекта

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)Найденный объект или null если объект не найден

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)