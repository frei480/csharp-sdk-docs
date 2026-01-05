

Руководство по T-FLEX CAD Open API

# GraphicsMoveTo - метод  
  
---  
  
Перемещение указателя в точку

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void MoveTo(
	Point point
)
```
```vb
Public Sub MoveTo ( 
	point As Point
)
```
```cpp
public:
void MoveTo(
	Point point
)
```


#### Параметры

point [Point](T_TFlex_Drawing_Point.md)
    Точка, в которую необходимо переместить указатель

Последующий вызов метода [LineTo(Point)](M_TFlex_Drawing_Graphics_LineTo.md) выведет отрезок, начинающийся в данной точке

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)