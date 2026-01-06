

Руководство по T-FLEX CAD Open API

# RoughnessSymbolSetRelativeLength - метод  
    
Установка типа и строк относительной опорной длины

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetRelativeLength(
	RoughnessRelativeLengthType parameterType,
	string minimum,
	string maximumOrNominal,
	string deviation,
	string p
)
```
```vb
Public Sub SetRelativeLength ( 
	parameterType As RoughnessRelativeLengthType,
	minimum As String,
	maximumOrNominal As String,
	deviation As String,
	p As String
)
```
```cpp
public:
void SetRelativeLength(
	RoughnessRelativeLengthType parameterType, 
	String^ minimum, 
	String^ maximumOrNominal, 
	String^ deviation, 
	String^ p
)
```


#### Параметры

parameterType [RoughnessRelativeLengthType](T_TFlex_Model_Model2D_RoughnessRelativeLengthType.md)
    Тип относительной опорной длины
minimum [String](https://learn.microsoft.com/dotnet/api/system.string)
    Минимум
maximumOrNominal [String](https://learn.microsoft.com/dotnet/api/system.string)
    Максимум или номинал
deviation [String](https://learn.microsoft.com/dotnet/api/system.string)
    Отклонения
p [String](https://learn.microsoft.com/dotnet/api/system.string)
    Параметр "p"

#### Ссылки

[RoughnessSymbol - ](T_TFlex_Model_Model2D_RoughnessSymbol.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)