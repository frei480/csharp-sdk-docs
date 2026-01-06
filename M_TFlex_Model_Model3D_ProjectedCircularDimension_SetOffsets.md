

Руководство по T-FLEX CAD Open API

# ProjectedCircularDimensionSetOffsets - метод  
    
Установка положения размера на окружности

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetOffsets(
	Node fixNode,
	double angle,
	double offset
)
```
```vb
Public Sub SetOffsets ( 
	fixNode As Node,
	angle As Double,
	offset As Double
)
```
```cpp
public:
void SetOffsets(
	Node^ fixNode, 
	double angle, 
	double offset
)
```


#### Параметры

fixNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел привязки размерной стрелки
angle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Угол, на котором находится размерная стрелка (используется, если отсутствует fixNode)
offset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Расстояние от размерного числа до окружности (используется, если отсутствует fixNode)

#### Ссылки

[ProjectedCircularDimension - ](T_TFlex_Model_Model3D_ProjectedCircularDimension.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)