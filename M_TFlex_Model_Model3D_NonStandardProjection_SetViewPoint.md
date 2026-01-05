

Руководство по T-FLEX CAD Open API

# NonStandardProjectionSetViewPoint - метод  
  
---  
  
Установить координаты точки проецирования

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetViewPoint(
	double xvp,
	double yvp,
	double zvp
)
```
```vb
Public Sub SetViewPoint ( 
	xvp As Double,
	yvp As Double,
	zvp As Double
)
```
```cpp
public:
void SetViewPoint(
	double xvp, 
	double yvp, 
	double zvp
)
```


#### Параметры

xvp [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Значение координаты x
yvp [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Значение координаты y
zvp [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Значение координаты z

Направление проецирования - вектор из заданной точки в (0., 0., 0.)

#### Ссылки

[NonStandardProjection - ](T_TFlex_Model_Model3D_NonStandardProjection.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)