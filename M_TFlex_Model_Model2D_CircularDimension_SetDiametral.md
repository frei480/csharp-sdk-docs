

Руководство по T-FLEX CAD Open API

# CircularDimensionSetDiametral - метод  
  
---  
  
Установка диаметрального размера

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetDiametral(
	Object2D circle,
	DiametralDimensionType type,
	Node fixNode,
	double angle,
	double offset
)
```
```vb
Public Sub SetDiametral ( 
	circle As Object2D,
	type As DiametralDimensionType,
	fixNode As Node,
	angle As Double,
	offset As Double
)
```
```cpp
public:
void SetDiametral(
	Object2D^ circle, 
	DiametralDimensionType type, 
	Node^ fixNode, 
	double angle, 
	double offset
)
```


#### Параметры

circle [Object2D](T_TFlex_Model_Model2D_Object2D.md)
    Окружность - линия построения или изображения, на которой устанавливается размер
type [DiametralDimensionType](T_TFlex_Model_Model2D_DiametralDimensionType.md)
    Тип отрисовки диаметрального размера
fixNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел привязки размерной стрелки
angle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Угол, на котором находится размерная стрелка (используется, если отсутствует fixNode)
offset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Расстояние от размерного числа до окружности (используется, если отсутствует fixNode)

#### Ссылки

[CircularDimension - ](T_TFlex_Model_Model2D_CircularDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)