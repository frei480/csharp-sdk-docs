

Руководство по T-FLEX CAD Open API

# ViewSearch(Double, Double, SelectionFilter, Double) - метод  
    
Поиск элемента модели

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ModelObject Search(
	double x,
	double y,
	SelectionFilter filter,
	double maxdist
)
```
```vb
Public Function Search ( 
	x As Double,
	y As Double,
	filter As SelectionFilter,
	maxdist As Double
) As ModelObject
```
```cpp
public:
ModelObject^ Search(
	double x, 
	double y, 
	SelectionFilter^ filter, 
	double maxdist
)
```


#### Параметры

x [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата X в модельных координатах
y [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата Y в модельных координатах
filter [SelectionFilter](T_TFlex_Model_SelectionFilter.md)
    Фильтр выбираемых объектов
maxdist [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Расстояние до объекта, пикселей

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)

#### Ссылки

[View - ](T_TFlex_Model_View.md)

[Search - перегрузка](Overload_TFlex_Model_View_Search.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)