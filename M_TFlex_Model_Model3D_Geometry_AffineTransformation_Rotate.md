

Руководство по T-FLEX CAD Open API

# AffineTransformationRotate - метод  
    
Вращение вокруг оси на заданный угол

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Rotate(
	BaseAxis axis,
	double angle
)
```
```vb
Public Sub Rotate ( 
	axis As BaseAxis,
	angle As Double
)
```
```cpp
public:
void Rotate(
	BaseAxis^ axis, 
	double angle
)
```


#### Параметры

axis [BaseAxis](T_TFlex_Model_Model3D_Geometry_BaseAxis.md)
    Ось, относительно которой выполняется вращение
angle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Угол в градусах, на который выполняется вращение

Вызов данного метода добавляет данное преобразование к уже заданным в этой трансформации

#### Ссылки

[AffineTransformation - ](T_TFlex_Model_Model3D_Geometry_AffineTransformation.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)