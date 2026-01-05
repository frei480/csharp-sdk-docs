

Руководство по T-FLEX CAD Open API

# RevolveArraySetRowParameters - метод  
  
---  
  
Установка параметров массива

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetRowParameters(
	RevolveArrayParameters paramsSet,
	Parameter arrFullAngle,
	Parameter arrStepAngle,
	Parameter arrNumber
)
```
```vb
Public Sub SetRowParameters ( 
	paramsSet As RevolveArrayParameters,
	arrFullAngle As Parameter,
	arrStepAngle As Parameter,
	arrNumber As Parameter
)
```
```cpp
public:
void SetRowParameters(
	RevolveArrayParameters paramsSet, 
	Parameter^ arrFullAngle, 
	Parameter^ arrStepAngle, 
	Parameter^ arrNumber
)
```


#### Параметры

paramsSet [RevolveArrayParameters](T_TFlex_Model_Model2D_RevolveArrayParameters.md)
    Набор параметров, которые устанавливаются функцией
arrFullAngle [Parameter](T_TFlex_Model_Parameter.md)
    Общая угол массива
arrStepAngle [Parameter](T_TFlex_Model_Parameter.md)
    Шаг угла для элементов
arrNumber [Parameter](T_TFlex_Model_Parameter.md)
    Количество элементов

В зависимости от заданного набора задаваемых параметров (paramsSet), оставшийся параметр будет автоматически рассчитываться по заданным двум (его значение, переданное в функцию будет проигнорировано). 

#### Ссылки

[RevolveArray - ](T_TFlex_Model_Model2D_RevolveArray.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)