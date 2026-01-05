

Руководство по T-FLEX CAD Open API

# LinearArraySetRowParameters - метод  
  
---  
  
Установка параметров рядов массива

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetRowParameters(
	LinearArrayParameters paramsSet,
	Parameter rowsLength,
	Parameter rowsStep,
	Parameter rowsNumber
)
```
```vb
Public Sub SetRowParameters ( 
	paramsSet As LinearArrayParameters,
	rowsLength As Parameter,
	rowsStep As Parameter,
	rowsNumber As Parameter
)
```
```cpp
public:
void SetRowParameters(
	LinearArrayParameters paramsSet, 
	Parameter^ rowsLength, 
	Parameter^ rowsStep, 
	Parameter^ rowsNumber
)
```


#### Параметры

paramsSet [LinearArrayParameters](T_TFlex_Model_Model2D_LinearArrayParameters.md)
    Набор параметров, которые устанавливаются функцией
rowsLength [Parameter](T_TFlex_Model_Parameter.md)
    Общая длина массива в направлении рядов
rowsStep [Parameter](T_TFlex_Model_Parameter.md)
    Шаг рядов
rowsNumber [Parameter](T_TFlex_Model_Parameter.md)
    Количество рядов

В зависимости от заданного набора задаваемых параметров (paramsSet), оставшийся параметр будет автоматически рассчитываться по заданным двум (его значение, переданное в функцию будет проигнорировано).

#### Ссылки

[LinearArray - ](T_TFlex_Model_Model2D_LinearArray.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)