

Руководство по T-FLEX CAD Open API

# ModelObjectSetReference(Int32, ModelObjectReference) - метод  
  
---  
  
Установить ссылку на родительcкий объект по ключу

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual void SetReference(
	int id,
	ModelObjectReference reference
)
```
```vb
Public Overridable Sub SetReference ( 
	id As Integer,
	reference As ModelObjectReference
)
```
```cpp
public:
virtual void SetReference(
	int id, 
	ModelObjectReference^ reference
)
```


#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор ключа, по которому в контейнере ссылок хранится объект
reference [ModelObjectReference](T_TFlex_Model_ModelObject_Reference.md)
    Ссылка на родительский объект

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[SetReference - перегрузка](Overload_TFlex_Model_ModelObject_SetReference.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)