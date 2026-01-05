

Руководство по T-FLEX CAD Open API

# DecorationCircleArc(String, BaseAxis, FloatVector, Double) - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public DecorationCircleArc(
	string name,
	BaseAxis axis,
	FloatVector start,
	double angle
)
```
```vb
Public Sub New ( 
	name As String,
	axis As BaseAxis,
	start As FloatVector,
	angle As Double
)
```
```cpp
public:
DecorationCircleArc(
	String^ name, 
	BaseAxis^ axis, 
	FloatVector start, 
	double angle
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя должно быть уникальным
axis [BaseAxis](T_TFlex_Model_Model3D_Geometry_BaseAxis.md)
    Ось
start [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Начало дуги
angle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Угол поворота в градусах

#### Значение поля

Создает дугу окружности по оси, началу дуги и углу 

#### Ссылки

[DecorationCircleArc - ](T_TFlex_Model_Model3D_Visual_DecorationCircleArc.md)

[DecorationCircleArc - перегрузка](Overload_TFlex_Model_Model3D_Visual_DecorationCircleArc__ctor.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)