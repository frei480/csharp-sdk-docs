

Руководство по T-FLEX CAD Open API

# CircularDimensionSetShortenedRadial - метод  
    
Установка радиального размера с изломом размерной линии

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetShortenedRadial(
	Object2D circle,
	Node fixAngleNode,
	double angle,
	double offset,
	Node fixRatioNode,
	double ratio,
	Node fixWidthNode,
	double width
)
```
```vb
Public Sub SetShortenedRadial ( 
	circle As Object2D,
	fixAngleNode As Node,
	angle As Double,
	offset As Double,
	fixRatioNode As Node,
	ratio As Double,
	fixWidthNode As Node,
	width As Double
)
```
```cpp
public:
void SetShortenedRadial(
	Object2D^ circle, 
	Node^ fixAngleNode, 
	double angle, 
	double offset, 
	Node^ fixRatioNode, 
	double ratio, 
	Node^ fixWidthNode, 
	double width
)
```


#### Параметры

circle [Object2D](T_TFlex_Model_Model2D_Object2D.md)
    Окружность - линия построения или изображения, на которой устанавливается размер
fixAngleNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел привязки размерной стрелки (привязка угла положения и начала стрелки)
angle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Угол, на котором находится размерная стрелка (используется, если отсутствует fixAngleNode)
offset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Расстояние от начала размерной линии до окружности (используется, если отсутствует fixAngleNode)
fixRatioNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел привязки положения излома размерной стрелки
ratio [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Соотношение, суммарной длины стрелки и длины стрелки после излома (используется, если отсутствует fixRatioNode)
fixWidthNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел привязки ширины излома размерной стрелки
width [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Ширина излома размерной стрелки (используется, если отсутствует fixWidthNode)

#### Ссылки

[CircularDimension - ](T_TFlex_Model_Model2D_CircularDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)