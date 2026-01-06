

Руководство по T-FLEX CAD Open API

# TermGroupMatch - метод  
    
Возвращает значение, указывающее, соответствует ли указанный объект условиям группы

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public override bool Match(
	Object obj
)
```
```vb
Public Overrides Function Match ( 
	obj As Object
) As Boolean
```
```cpp
public:
virtual bool Match(
	Object^ obj
) override
```


#### Параметры

obj [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Объект для проверки

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Значение true, если объект соответствует условиям группы; в противном случае - значение false

#### Ссылки

[TermGroup - ](T_TFlex_Model_Data_Filters_TermGroup.md)

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)