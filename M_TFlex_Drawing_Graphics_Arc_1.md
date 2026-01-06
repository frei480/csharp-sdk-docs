

Руководство по T-FLEX CAD Open API

# GraphicsArc(Point, Point, Point, Boolean) - метод  
    
Прорисовка дуги с центром в заданной точке, проходящей через две точки

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Arc(
	Point center,
	Point point1,
	Point point2,
	bool direction
)
```




#### Параметры

center [Point](T_TFlex_Drawing_Point.md)
    Центральная точка дуги
point1 [Point](T_TFlex_Drawing_Point.md)
    Точка начала дуги
point2 [Point](T_TFlex_Drawing_Point.md)
    Точка конца дуги
direction [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Направление дуги. При значении true против часовой стрелки; false - по часовой стрелке

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[Arc - перегрузка](Overload_TFlex_Drawing_Graphics_Arc.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)