

Руководство по T-FLEX CAD Open API

# DynamicStudySolve(DynamicStudySolveCallback) - метод  
  
---  
  
Рассчитать задачу с возможностью досрочной остановки расчёта

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool Solve(
	DynamicStudySolveCallback callback
)
```
```vb
Public Function Solve ( 
	callback As DynamicStudySolveCallback
) As Boolean
```
```cpp
public:
bool Solve(
	DynamicStudySolveCallback^ callback
)
```


#### Параметры

callback [DynamicStudySolveCallback](T_TFlex_Model_Model3D_DynamicStudy_SolveCallback.md)
    Функция, вызываемая в конце каждого шага симуляции. Возврат значения false сигнализирует о необходимости прервать расчёт

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Функция, переданная в параметре callback, не должна каким-либо образом изменять состояние относящихся к задаче объектов, так как это может привести к нежелательным последствиям

#### Ссылки

[DynamicStudy - ](T_TFlex_Model_Model3D_DynamicStudy.md)

[Solve - перегрузка](Overload_TFlex_Model_Model3D_DynamicStudy_Solve.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)