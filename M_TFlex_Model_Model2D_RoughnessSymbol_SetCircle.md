

Руководство по T-FLEX CAD Open API

# RoughnessSymbolSetCircle - метод  
    
Установка параметров привязки к окружности

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetCircle(
	Object2D circle,
	Parameter cosAngle,
	Parameter sinAngle
)
```
```vb
Public Sub SetCircle ( 
	circle As Object2D,
	cosAngle As Parameter,
	sinAngle As Parameter
)
```
```cpp
public:
void SetCircle(
	Object2D^ circle, 
	Parameter^ cosAngle, 
	Parameter^ sinAngle
)
```


#### Параметры

circle [Object2D](T_TFlex_Model_Model2D_Object2D.md)
    Окружность привязки
cosAngle [Parameter](T_TFlex_Model_Parameter.md)
    Косинус угла, на котором находится точка привязки
sinAngle [Parameter](T_TFlex_Model_Parameter.md)
    Синус угла, на котором находится точка привязки

#### Ссылки

[RoughnessSymbol - ](T_TFlex_Model_Model2D_RoughnessSymbol.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)