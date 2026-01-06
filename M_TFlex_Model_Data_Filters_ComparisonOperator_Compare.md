

Руководство по T-FLEX CAD Open API

# ComparisonOperatorCompare - метод  
    
Возвращает значение, указывающее, выполняется ли условие оператора сравнения для указанных операндов

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public abstract bool Compare(
	Object firstOperand,
	Object secondOperand
)
```
```vb
Public MustOverride Function Compare ( 
	firstOperand As Object,
	secondOperand As Object
) As Boolean
```
```cpp
public:
virtual bool Compare(
	Object^ firstOperand, 
	Object^ secondOperand
) abstract
```


#### Параметры

firstOperand [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Первый операнд
secondOperand [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Второй операнд

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Значение true, если условие оператора выполняется для указанных операндов; в противном случае - значение false

#### Ссылки

[ComparisonOperator - ](T_TFlex_Model_Data_Filters_ComparisonOperator.md)

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)