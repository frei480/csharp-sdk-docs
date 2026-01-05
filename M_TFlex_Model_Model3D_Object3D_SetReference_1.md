

Руководство по T-FLEX CAD Open API

# Object3DSetReference(Int32, ModelObjectReference, ModelObjectArrayIndices) - метод  
  
---  
  
Установить ссылку на родительский объект по ключу и индексу

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public override void SetReference(
	int id,
	ModelObjectReference reference,
	ModelObjectArrayIndices indices
)
```
```vb
Public Overrides Sub SetReference ( 
	id As Integer,
	reference As ModelObjectReference,
	indices As ModelObjectArrayIndices
)
```
```cpp
public:
virtual void SetReference(
	int id, 
	ModelObjectReference^ reference, 
	ModelObjectArrayIndices^ indices
) override
```


#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор ключа, по которому в контейнере ссылок хранится объект
reference [ModelObjectReference](T_TFlex_Model_ModelObject_Reference.md)
    Ссылка на родительский объект
indices [ModelObjectArrayIndices](T_TFlex_Model_ModelObject_ArrayIndices.md)
    Координаты элемента

Используется для организации массивов

#### Ссылки

[Object3D - ](T_TFlex_Model_Model3D_Object3D.md)

[SetReference - перегрузка](Overload_TFlex_Model_Model3D_Object3D_SetReference.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)