

Руководство по T-FLEX CAD Open API

# FormlimitsLeaderSetDimension - метод  
  
---  
  
Установка привязки к размеру

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetDimension(
	Dimension dim,
	bool isOnEnd
)
```
```vb
Public Sub SetDimension ( 
	dim As Dimension,
	isOnEnd As Boolean
)
```
```cpp
public:
void SetDimension(
	Dimension^ dim, 
	bool isOnEnd
)
```


#### Параметры

dim [Dimension](T_TFlex_Model_Model2D_Dimension.md)
    Размер привязки
isOnEnd [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Значение true указывает, что привязка выполняется к концу размера, false - к началу

#### Ссылки

[FormlimitsLeader - ](T_TFlex_Model_Model2D_FormlimitsLeader.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)