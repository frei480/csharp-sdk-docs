

Руководство по T-FLEX CAD Open API

# CircularDimensionSetRadial - метод  
  
---  
  
Установка радиального размера

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetRadial(
	Object2D circle,
	RadialDimensionType type,
	Node fixNode,
	double angle,
	double offset
)
```
```vb
Public Sub SetRadial ( 
	circle As Object2D,
	type As RadialDimensionType,
	fixNode As Node,
	angle As Double,
	offset As Double
)
```
```cpp
public:
void SetRadial(
	Object2D^ circle, 
	RadialDimensionType type, 
	Node^ fixNode, 
	double angle, 
	double offset
)
```


#### Параметры

circle [Object2D](T_TFlex_Model_Model2D_Object2D.md)
    Окружность - линия построения или изображения, на которой устанавливается размер
type [RadialDimensionType](T_TFlex_Model_Model2D_RadialDimensionType.md)
    Тип отрисовки радиального размера
fixNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел привязки размерной стрелки
angle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Угол, на котором находится размерная стрелка (используется, если отсутствует fixNode)
offset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Расстояние от размерного числа до окружности (используется, если отсутствует fixNode)

#### Ссылки

[CircularDimension - ](T_TFlex_Model_Model2D_CircularDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)