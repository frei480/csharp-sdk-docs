

Руководство по T-FLEX CAD Open API

# TermGroupItemMatch - метод  
    
Возвращает значение, указывающее, соответствует ли указанный объект условиям текущего элемента

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public abstract bool Match(
	Object obj
)
```
```vb
Public MustOverride Function Match ( 
	obj As Object
) As Boolean
```
```cpp
public:
virtual bool Match(
	Object^ obj
) abstract
```


#### Параметры

obj [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Объект для проверки

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Значение true, если объект соответствует условиям текущего элемента; в противном случае - значение false

#### Ссылки

[TermGroupItem - ](T_TFlex_Model_Data_Filters_TermGroupItem.md)

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)