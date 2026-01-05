

Руководство по T-FLEX CAD Open API

# LineConstructionSetTangentToCircleOnAngle - метод  
  
---  
  
Прямая, касательная к окружности, под углом к другой прямой

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToCircleOnAngle(
	Construction srcLine,
	Construction srcCircle,
	int variant,
	Parameter angle
)
```
```vb
Public Sub SetTangentToCircleOnAngle ( 
	srcLine As Construction,
	srcCircle As Construction,
	variant As Integer,
	angle As Parameter
)
```
```cpp
public:
void SetTangentToCircleOnAngle(
	Construction^ srcLine, 
	Construction^ srcCircle, 
	int variant, 
	Parameter^ angle
)
```


#### Параметры

srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная прямая
srcCircle [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная окружность
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта прямой
angle [Parameter](T_TFlex_Model_Parameter.md)
    Значение угла в градусах

#### Ссылки

[LineConstruction - ](T_TFlex_Model_Model2D_LineConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)