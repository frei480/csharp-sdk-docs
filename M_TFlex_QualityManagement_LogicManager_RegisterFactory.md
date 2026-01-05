

Руководство по T-FLEX CAD Open API

# LogicManagerRegisterFactory - метод  
  
---  
  
Зарегистрировать фабрику логик

**Пространство имён:** [TFlex.QualityManagement](N_TFlex_QualityManagement.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool RegisterFactory(
	Guid logicUid,
	ILogicFactory factory
)
```
```vb
Public Function RegisterFactory ( 
	logicUid As Guid,
	factory As ILogicFactory
) As Boolean
```
```cpp
public:
bool RegisterFactory(
	Guid logicUid, 
	ILogicFactory^ factory
)
```


#### Параметры

logicUid [Guid](https://learn.microsoft.com/dotnet/api/system.guid)
    
factory [ILogicFactory](T_TFlex_QualityManagement_ILogicFactory.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[LogicManager - ](T_TFlex_QualityManagement_LogicManager.md)

[TFlex.QualityManagement - пространство имён](N_TFlex_QualityManagement.md)