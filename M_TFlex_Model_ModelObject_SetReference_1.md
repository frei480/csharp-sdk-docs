

Руководство по T-FLEX CAD Open API

# ModelObjectSetReference(Int32, ModelObjectReference, ModelObjectArrayIndices) - метод  
    
Установить ссылку на родительский объект по ключу и индексу. Используется для организации массивов

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual void SetReference(
	int id,
	ModelObjectReference reference,
	ModelObjectArrayIndices indices
)
```




#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор ключа, по которому в контейнере ссылок хранится объект
reference [ModelObjectReference](T_TFlex_Model_ModelObject_Reference.md)
    Ссылка на родительский объект
indices [ModelObjectArrayIndices](T_TFlex_Model_ModelObject_ArrayIndices.md)
    Координаты элемента

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[SetReference - перегрузка](Overload_TFlex_Model_ModelObject_SetReference.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)