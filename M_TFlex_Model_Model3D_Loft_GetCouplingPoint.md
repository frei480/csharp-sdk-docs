

Руководство по T-FLEX CAD Open API

# LoftGetCouplingPoint - метод  
  
---  
  
Задать точку соответствия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public LoftPointOnContour GetCouplingPoint(
	int couplingIndex,
	int profileIndex
)
```
```vb
Public Function GetCouplingPoint ( 
	couplingIndex As Integer,
	profileIndex As Integer
) As LoftPointOnContour
```
```cpp
public:
LoftPointOnContour^ GetCouplingPoint(
	int couplingIndex, 
	int profileIndex
)
```


#### Параметры

couplingIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс последовательности точек соответствия
profileIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс точки в последовательности точек соответствия.

#### Возвращаемое значение

[LoftPointOnContour](T_TFlex_Model_Model3D_Loft_PointOnContour.md)Точка лежащая на соответствующем профиле

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

[RemoveCoupling(Int32)](M_TFlex_Model_Model3D_Loft_RemoveCoupling.md)

[ResetCouplingPoint(Int32, Int32)](M_TFlex_Model_Model3D_Loft_ResetCouplingPoint.md)