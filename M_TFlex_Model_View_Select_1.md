

Руководство по T-FLEX CAD Open API

# ViewSelect(Point, SelectionFilter) - метод  
  
---  
  
Выбор элемента модели

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

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
    Точка в координатах экрана
filter [SelectionFilter](T_TFlex_Model_SelectionFilter.md)
    Фильтр выбираемых объектов

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)

#### Ссылки

[View - ](T_TFlex_Model_View.md)

[Select - перегрузка](Overload_TFlex_Model_View_Select.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)