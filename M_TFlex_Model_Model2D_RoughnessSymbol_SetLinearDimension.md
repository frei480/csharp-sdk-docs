

Руководство по T-FLEX CAD Open API

# RoughnessSymbolSetLinearDimension - метод  
  
---  
  
Установка параметров привязки к линейному размеру

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetLinearDimension(
	LinearDimension dim,
	bool onSecondLine,
	Parameter offset
)
```
```vb
Public Sub SetLinearDimension ( 
	dim As LinearDimension,
	onSecondLine As Boolean,
	offset As Parameter
)
```
```cpp
public:
void SetLinearDimension(
	LinearDimension^ dim, 
	bool onSecondLine, 
	Parameter^ offset
)
```


#### Параметры

dim [LinearDimension](T_TFlex_Model_Model2D_LinearDimension.md)
    Размер для привязки
onSecondLine [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Параметр, к какой из линий размера осуществлять привязку
offset [Parameter](T_TFlex_Model_Parameter.md)
    Смещение положения точки привязки от размерной линии

#### Ссылки

[RoughnessSymbol - ](T_TFlex_Model_Model2D_RoughnessSymbol.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)