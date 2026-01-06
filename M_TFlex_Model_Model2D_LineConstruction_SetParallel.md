

Руководство по T-FLEX CAD Open API

# LineConstructionSetParallel - метод  
    
Параллельная прямая

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetParallel(
	Construction srcLine,
	Parameter distance
)
```
```vb
Public Sub SetParallel ( 
	srcLine As Construction,
	distance As Parameter
)
```
```cpp
public:
void SetParallel(
	Construction^ srcLine, 
	Parameter^ distance
)
```


#### Параметры

srcLine [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная линия построения (прямая)
distance [Parameter](T_TFlex_Model_Parameter.md)
    Устанавливаемое значение расстояния

Функция устанавливает параметры линии построения, соответствующие прямой, параллельной исходной прямой. Прямая располагается на расстоянии distance от исходной прямой (без учёта масштаба текущей страницы).

#### Ссылки

[LineConstruction - ](T_TFlex_Model_Model2D_LineConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)