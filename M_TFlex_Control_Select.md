

Руководство по T-FLEX CAD Open API

# ControlSelect(Point, SelectionFilter) - метод  
    
Выбор элемента модели, ближайшего к заданной точке

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ModelObject Select(
	Point point,
	SelectionFilter filter
)
```
```vb
Public Function Select ( 
	point As Point,
	filter As SelectionFilter
) As ModelObject
```
```cpp
public:
ModelObject^ Select(
	Point point, 
	SelectionFilter^ filter
)
```


#### Параметры

point [Point](https://learn.microsoft.com/dotnet/api/system.drawing.point)
    Точка на экране
filter [SelectionFilter](T_TFlex_Model_SelectionFilter.md)
    Фильтр выбора объектов

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)

#### Ссылки

[Control - ](T_TFlex_Control.md)

[Select - перегрузка](Overload_TFlex_Control_Select.md)

[TFlex - пространство имён](N_TFlex.md)