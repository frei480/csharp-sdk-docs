

Руководство по T-FLEX CAD Open API

# GraphicsArrowLine - метод  
    
Прорисовка отрезка со стрелками

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void ArrowLine(
	Point start,
	Point end,
	int startType,
	double startSize,
	int endType,
	double endSize
)
```
```vb
Public Sub ArrowLine ( 
	start As Point,
	end As Point,
	startType As Integer,
	startSize As Double,
	endType As Integer,
	endSize As Double
)
```
```cpp
public:
void ArrowLine(
	Point start, 
	Point end, 
	int startType, 
	double startSize, 
	int endType, 
	double endSize
)
```


#### Параметры

start [Point](T_TFlex_Drawing_Point.md)
    Начальная точка отрезка
end [Point](T_TFlex_Drawing_Point.md)
    Конечная точка отрезка
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