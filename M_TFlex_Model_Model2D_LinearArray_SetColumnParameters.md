

Руководство по T-FLEX CAD Open API

# LinearArraySetColumnParameters - метод  
    
Установка параметров столбцов массива

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetColumnParameters(
	LinearArrayParameters paramsSet,
	NodeNeeds nodeNeed,
	Parameter colsLength,
	Parameter colsStep,
	Parameter colsNumber
)
```
```vb
Public Sub SetColumnParameters ( 
	paramsSet As LinearArrayParameters,
	nodeNeed As NodeNeeds,
	colsLength As Parameter,
	colsStep As Parameter,
	colsNumber As Parameter
)
```
```cpp
public:
void SetColumnParameters(
	LinearArrayParameters paramsSet, 
	NodeNeeds nodeNeed, 
	Parameter^ colsLength, 
	Parameter^ colsStep, 
	Parameter^ colsNumber
)
```


#### Параметры

paramsSet [LinearArrayParameters](T_TFlex_Model_Model2D_LinearArrayParameters.md)
    Набор параметров, которые устанавливаются функцией
nodeNeed [NodeNeeds](T_TFlex_Model_Model2D_NodeNeeds.md)
    Указывает способ использования конечной точка
colsLength [Parameter](T_TFlex_Model_Parameter.md)
    Общая длина массива в направлении столбцов
colsStep [Parameter](T_TFlex_Model_Parameter.md)
    Шаг столбцов
colsNumber [Parameter](T_TFlex_Model_Parameter.md)
    Количество столбцов

В зависимости от заданного набора задаваемых параметров (paramsSet), оставшийся параметр будет автоматически рассчитываться по заданным двум (его значение, переданное в функцию будет проигнорировано). В зависимости от заданного флага узла (nodeNeed), переданное в функцию значение параметра, получаемого с узла, будет проигнорировано. При попытке указать для получения по конечной точке привязки расчитываемого значения, nodeNeed будет автоматически установлен в None.

#### Ссылки

[LinearArray - ](T_TFlex_Model_Model2D_LinearArray.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)