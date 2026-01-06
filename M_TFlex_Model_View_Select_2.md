

Руководство по T-FLEX CAD Open API

# ViewSelect(Int32, Int32, SelectionFilter) - метод  
    
Выбор элемента модели

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ModelObject Select(
	int x,
	int y,
	SelectionFilter filter
)
```
```vb
Public Function Select ( 
	x As Integer,
	y As Integer,
	filter As SelectionFilter
) As ModelObject
```
```cpp
public:
ModelObject^ Select(
	int x, 
	int y, 
	SelectionFilter^ filter
)
```


#### Параметры

x [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Координата X курсора
y [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Координата Y курсора
filter [SelectionFilter](T_TFlex_Model_SelectionFilter.md)
    Фильтр выбираемых объектов

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)

#### Ссылки

[View - ](T_TFlex_Model_View.md)

[Select - перегрузка](Overload_TFlex_Model_View_Select.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)