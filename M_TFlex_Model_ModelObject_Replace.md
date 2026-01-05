

Руководство по T-FLEX CAD Open API

# ModelObjectReplace - метод  
  
---  
  
Заменить объект

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool Replace(
	ModelObject source,
	bool deleteSource
)
```
```vb
Public Function Replace ( 
	source As ModelObject,
	deleteSource As Boolean
) As Boolean
```
```cpp
public:
bool Replace(
	ModelObject^ source, 
	bool deleteSource
)
```


#### Параметры

source [ModelObject](T_TFlex_Model_ModelObject.md)
    Исходный объект, который нужно заменить
deleteSource [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Удалить заменённый объект после замены

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)