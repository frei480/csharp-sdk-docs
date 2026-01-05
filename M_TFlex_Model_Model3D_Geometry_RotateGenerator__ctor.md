

Руководство по T-FLEX CAD Open API

# RotateGenerator - конструктор  
  
---  
  
Конструктор для задания вращения

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public RotateGenerator(
	ProxyObject3D object,
	BaseAxis axis,
	Body profile,
	double angle
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	axis As BaseAxis,
	profile As Body,
	angle As Double
)
```
```cpp
public:
RotateGenerator(
	ProxyObject3D^ object, 
	BaseAxis^ axis, 
	Body^ profile, 
	double angle
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
axis [BaseAxis](T_TFlex_Model_Model3D_Geometry_BaseAxis.md)
    Ось вращения
profile [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Вращаемый контур. Этот контур превращается во вращение и возращается в списке результирующих тел или удаляется
angle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Угол поворота

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[RotateGenerator - ](T_TFlex_Model_Model3D_Geometry_RotateGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)