

Руководство по T-FLEX CAD Open API

# LineConstructionSetHorizontal - метод  
    
Горизонтальная прямая

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetHorizontal(
	Parameter distance
)
```
```vb
Public Sub SetHorizontal ( 
	distance As Parameter
)
```
```cpp
public:
void SetHorizontal(
	Parameter^ distance
)
```


#### Параметры

distance [Parameter](T_TFlex_Model_Parameter.md)
    Устанавливаемое значение координаты Y

Функция устанавливает параметры линии построения, соответствующие горизонтальной прямой. Прямая располагается на расстоянии distance от оси X системы координат модели (без учёта масштаба текущей страницы)

#### Ссылки

[LineConstruction - ](T_TFlex_Model_Model2D_LineConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)