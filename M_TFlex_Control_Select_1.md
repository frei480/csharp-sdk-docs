

Руководство по T-FLEX CAD Open API

# ControlSelect(Int32, Int32, SelectionFilter) - метод  
  
---  
  
Выбор элемента модели, ближайшего к точке с заданными координатами

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual ModelObject Select(
	int x,
	int y,
	SelectionFilter filter
)
```
```vb
Public Overridable Function Select ( 
	x As Integer,
	y As Integer,
	filter As SelectionFilter
) As ModelObject
```
```cpp
public:
virtual ModelObject^ Select(
	int x, 
	int y, 
	SelectionFilter^ filter
)
```


#### Параметры

x [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Координата X в экранной системе координат
y [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Координата Y в экранной системе координат
filter [SelectionFilter](T_TFlex_Model_SelectionFilter.md)
    Фильтр выбора объектов

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)

#### Ссылки

[Control - ](T_TFlex_Control.md)

[Select - перегрузка](Overload_TFlex_Control_Select.md)

[TFlex - пространство имён](N_TFlex.md)