

Руководство по T-FLEX CAD Open API

# GraphicsLineTo - метод  
  
---  
  
Прорисовка отрезка от указателя к данной точке

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void LineTo(
	Point point
)
```
```vb
Public Sub LineTo ( 
	point As Point
)
```
```cpp
public:
void LineTo(
	Point point
)
```


#### Параметры

point [Point](T_TFlex_Drawing_Point.md)
    Точка, в которую необходимо провести отрезок и переместить указатель

Отрезок выводится от указателя, который был установлен методом [MoveTo(Point)](M_TFlex_Drawing_Graphics_MoveTo.md) или предыдущим вызовом метода LineTo(Point)

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)