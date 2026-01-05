

Руководство по T-FLEX CAD Open API

# DecorationNURBS(String, BasePoint3D, Double, Double) - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public DecorationNURBS(
	string name,
	BasePoint3D[] controlPoints,
	double[] weights,
	double[] knots
)
```
```vb
Public Sub New ( 
	name As String,
	controlPoints As BasePoint3D(),
	weights As Double(),
	knots As Double()
)
```
```cpp
public:
DecorationNURBS(
	String^ name, 
	array<BasePoint3D^>^ controlPoints, 
	array<double>^ weights, 
	array<double>^ knots
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя должно быть уникальным
controlPoints [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    Определяющие точки
weights [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Веса точек
knots [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Узловой вектор

Число элементов массивов weights и controlPoints должно совпадать 

#### Ссылки

[DecorationNURBS - ](T_TFlex_Model_Model3D_Visual_DecorationNURBS.md)

[DecorationNURBS - перегрузка](Overload_TFlex_Model_Model3D_Visual_DecorationNURBS__ctor.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)