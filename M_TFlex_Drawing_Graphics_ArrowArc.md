

Руководство по T-FLEX CAD Open API

# GraphicsArrowArc - метод  
    
Прорисовка дуги со стрелками с центром в заданной точке, проходящей через две точки, против часовой стрелки

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void ArrowArc(
	Point center,
	Point point1,
	Point point2,
	int startType,
	double startSize,
	int endType,
	double endSize
)
```
```vb
Public Sub ArrowArc ( 
	center As Point,
	point1 As Point,
	point2 As Point,
	startType As Integer,
	startSize As Double,
	endType As Integer,
	endSize As Double
)
```
```cpp
public:
void ArrowArc(
	Point center, 
	Point point1, 
	Point point2, 
	int startType, 
	double startSize, 
	int endType, 
	double endSize
)
```


#### Параметры

center [Point](T_TFlex_Drawing_Point.md)
    Центральная точка дуги
point1 [Point](T_TFlex_Drawing_Point.md)
    Точка начала дуги
point2 [Point](T_TFlex_Drawing_Point.md)
    Точка конца дуги
startType [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Тип стрелки в начальной точке
startSize [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Размер стрелки в начальной точке
endType [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Тип стрелки в конечной точке
endSize [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Размер стрелки в конечной точке

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)