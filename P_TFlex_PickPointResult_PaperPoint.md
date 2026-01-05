

Руководство по T-FLEX CAD Open API

# PickPointResultPaperPoint - свойство  
  
---  
  
Выбранная точка в системе координат бумаги, без учёта масштаба текущей страницы

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Point PaperPoint { get; set; }
```
```vb
Public Property PaperPoint As Point
	Get
	Set
```
```cpp
public:
property Point PaperPoint {
	Point get ();
	void set (Point value);
}
```


#### Значение свойства

[Point](T_TFlex_Drawing_Point.md)

Данный параметр имеет смысл только в случае выбора точки в 2D виде или в 3D виде в режиме активизации страницы рабочей плоскости.

#### Ссылки

[PickPointResult - ](T_TFlex_PickPointResult.md)

[TFlex - пространство имён](N_TFlex.md)