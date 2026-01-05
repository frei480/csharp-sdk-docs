

Руководство по T-FLEX CAD Open API

# AffineTransformationScale - метод  
  
---  
  
Масштабирование по осям глобальной системы координат

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Scale(
	double xscale,
	double yscale,
	double zscale
)
```
```vb
Public Sub Scale ( 
	xscale As Double,
	yscale As Double,
	zscale As Double
)
```
```cpp
public:
void Scale(
	double xscale, 
	double yscale, 
	double zscale
)
```


#### Параметры

xscale [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Масштаб по оси X
yscale [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Масштаб по оси Y
zscale [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Масштаб по оси Z

Вызов данного метода добавляет данное преобразование к уже заданным в этой трансформации

#### Ссылки

[AffineTransformation - ](T_TFlex_Model_Model3D_Geometry_AffineTransformation.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)