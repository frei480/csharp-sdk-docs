

Руководство по T-FLEX CAD Open API

# RoughnessSymbolSetStepParameter - метод  
  
---  
  
Установка типа и строк шагового параметра

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetStepParameter(
	RoughnessStepParameterType parameterType,
	string minimum,
	string maximumOrNominal,
	string deviation,
	string basicLength
)
```
```vb
Public Sub SetStepParameter ( 
	parameterType As RoughnessStepParameterType,
	minimum As String,
	maximumOrNominal As String,
	deviation As String,
	basicLength As String
)
```
```cpp
public:
void SetStepParameter(
	RoughnessStepParameterType parameterType, 
	String^ minimum, 
	String^ maximumOrNominal, 
	String^ deviation, 
	String^ basicLength
)
```


#### Параметры

parameterType [RoughnessStepParameterType](T_TFlex_Model_Model2D_RoughnessStepParameterType.md)
    Тип шагового параметра
minimum [String](https://learn.microsoft.com/dotnet/api/system.string)
    Минимум
maximumOrNominal [String](https://learn.microsoft.com/dotnet/api/system.string)
    Максимум или номинал
deviation [String](https://learn.microsoft.com/dotnet/api/system.string)
    Отклонение
basicLength [String](https://learn.microsoft.com/dotnet/api/system.string)
    Базовая длина

#### Ссылки

[RoughnessSymbol - ](T_TFlex_Model_Model2D_RoughnessSymbol.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)