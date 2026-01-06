

Руководство по T-FLEX CAD Open API

# DecorationNURBS(String, FloatVector, Single, Single) - конструктор  
    
Конструктор

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public DecorationNURBS(
	string name,
	FloatVector[] controlPoints,
	float[] weights,
	float[] knots
)
```
```vb
Public Sub New ( 
	name As String,
	controlPoints As FloatVector(),
	weights As Single(),
	knots As Single()
)
```
```cpp
public:
DecorationNURBS(
	String^ name, 
	array<FloatVector>^ controlPoints, 
	array<float>^ weights, 
	array<float>^ knots
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя должно быть уникальным
controlPoints [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Определяющие точки
weights [Single](https://learn.microsoft.com/dotnet/api/system.single)
    Веса точек
knots [Single](https://learn.microsoft.com/dotnet/api/system.single)
    Узловой вектор

Число элементов массивов weights и controlPoints должно совпадать 

#### Ссылки

[DecorationNURBS - ](T_TFlex_Model_Model3D_Visual_DecorationNURBS.md)

[DecorationNURBS - перегрузка](Overload_TFlex_Model_Model3D_Visual_DecorationNURBS__ctor.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)