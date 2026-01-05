

Руководство по T-FLEX CAD Open API

# OperationFindBodyOwner - метод  
  
---  
  
Получить базовую операцию, в которой хранятся свойства тела

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Operation FindBodyOwner(
	bool any
)
```
```vb
Public Function FindBodyOwner ( 
	any As Boolean
) As Operation
```
```cpp
public:
Operation^ FindBodyOwner(
	bool any
)
```


#### Параметры

any [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Если базовой операции нет, то возвращать саму передаваемую операцию

#### Возвращаемое значение

[Operation](T_TFlex_Model_Model3D_Operation.md)

#### Ссылки

[Operation - ](T_TFlex_Model_Model3D_Operation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)