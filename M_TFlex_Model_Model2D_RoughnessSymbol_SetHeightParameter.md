

Руководство по T-FLEX CAD Open API

# RoughnessSymbolSetHeightParameter - метод  
    
Установка типа и строк высотного параметра

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetHeightParameter(
	RoughnessHeightParameterType parameterType,
	string minimum,
	string maximumOrNominal,
	string deviation,
	string basicLength
)
```
```vb
Public Sub SetHeightParameter ( 
	parameterType As RoughnessHeightParameterType,
	minimum As String,
	maximumOrNominal As String,
	deviation As String,
	basicLength As String
)
```
```cpp
public:
void SetHeightParameter(
	RoughnessHeightParameterType parameterType, 
	String^ minimum, 
	String^ maximumOrNominal, 
	String^ deviation, 
	String^ basicLength
)
```


#### Параметры

parameterType [RoughnessHeightParameterType](T_TFlex_Model_Model2D_RoughnessHeightParameterType.md)
    Тип высотного параметра
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