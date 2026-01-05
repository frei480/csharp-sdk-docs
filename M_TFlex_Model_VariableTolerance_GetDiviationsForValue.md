

Руководство по T-FLEX CAD Open API

# VariableToleranceGetDiviationsForValue - метод  
  
---  
**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool GetDiviationsForValue(
	double value,
	out double lower,
	out double upper
)
```
```vb
Public Function GetDiviationsForValue ( 
	value As Double,
	<OutAttribute> ByRef lower As Double,
	<OutAttribute> ByRef upper As Double
) As Boolean
```
```cpp
public:
bool GetDiviationsForValue(
	double value, 
	[OutAttribute] double% lower, 
	[OutAttribute] double% upper
)
```


#### Параметры

value [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
lower [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
upper [Double](https://learn.microsoft.com/dotnet/api/system.double)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[VariableTolerance - ](T_TFlex_Model_VariableTolerance.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)