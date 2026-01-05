

Руководство по T-FLEX CAD Open API

# BaseCurveDerivative - метод  
  
---  
  
Вычислить производные в точке на кривой по параметру

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Direction[] Derivative(
	double t,
	uint derivative
)
```
```vb
Public Function Derivative ( 
	t As Double,
	derivative As UInteger
) As Direction()
```
```cpp
public:
array<Direction^>^ Derivative(
	double t, 
	unsigned int derivative
)
```


#### Параметры

t [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Параметр
derivative [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Максимальный порядок производной

#### Возвращаемое значение

[Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)

#### Ссылки

[BaseCurve - ](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)