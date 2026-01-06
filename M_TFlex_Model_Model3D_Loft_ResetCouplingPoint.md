

Руководство по T-FLEX CAD Open API

# LoftResetCouplingPoint - метод  
    
Задать точку соответствия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void ResetCouplingPoint(
	int couplingIndex,
	int profileIndex
)
```
```vb
Public Sub ResetCouplingPoint ( 
	couplingIndex As Integer,
	profileIndex As Integer
)
```
```cpp
public:
void ResetCouplingPoint(
	int couplingIndex, 
	int profileIndex
)
```


#### Параметры

couplingIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс последовательности точек соответствия
profileIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс точки в последовательности точек соответствия.

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

[RemoveCoupling(Int32)](M_TFlex_Model_Model3D_Loft_RemoveCoupling.md)

ResetCouplingPoint(Int32, Int32)