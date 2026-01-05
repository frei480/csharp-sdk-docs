

Руководство по T-FLEX CAD Open API

# LineConstructionSetAxisOfLines - метод  
  
---  
  
Прямая, являющаяся осью симметрии двух прямых

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetAxisOfLines(
	Construction srcLine1,
	Construction srcLine2,
	int variant
)
```
```vb
Public Sub SetAxisOfLines ( 
	srcLine1 As Construction,
	srcLine2 As Construction,
	variant As Integer
)
```
```cpp
public:
void SetAxisOfLines(
	Construction^ srcLine1, 
	Construction^ srcLine2, 
	int variant
)
```


#### Параметры

srcLine1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая исходная прямая
srcLine2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая исходная прямая
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта прямой

#### Ссылки

[LineConstruction - ](T_TFlex_Model_Model2D_LineConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)