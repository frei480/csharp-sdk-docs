

Руководство по T-FLEX CAD Open API

# PickPointResultModelPoint - свойство  
    
Выбранная точка в системе координат модели, с учётом масштаба текущей страницы

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Point ModelPoint { get; }
```
```vb
Public ReadOnly Property ModelPoint As Point
	Get
```
```cpp
public:
property Point ModelPoint {
	Point get ();
}
```


#### Значение свойства

[Point](T_TFlex_Drawing_Point.md)

Данный параметр имеет смысл только в случае выбора точки в 2D виде или в 3D виде в режиме активизации страницы рабочей плоскости.

#### Ссылки

[PickPointResult - ](T_TFlex_PickPointResult.md)

[TFlex - пространство имён](N_TFlex.md)