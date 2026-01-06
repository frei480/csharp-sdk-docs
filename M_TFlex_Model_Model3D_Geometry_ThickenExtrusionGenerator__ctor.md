

Руководство по T-FLEX CAD Open API

# ThickenExtrusionGenerator - конструктор  
    
Конструктор для задания придания толщины

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ThickenExtrusionGenerator(
	ProxyObject3D object,
	Body sheet,
	double thickness,
	double backThickness
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	sheet As Body,
	thickness As Double,
	backThickness As Double
)
```
```cpp
public:
ThickenExtrusionGenerator(
	ProxyObject3D^ object, 
	Body^ sheet, 
	double thickness, 
	double backThickness
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
sheet [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Листовое тело. Этот лист возращается в списке результирующих тел или удаляется
thickness [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Величина толщины в лицевом направлении
backThickness [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Величина толщины в изнаночном направлении

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[ThickenExtrusionGenerator - ](T_TFlex_Model_Model3D_Geometry_ThickenExtrusionGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)