

Руководство по T-FLEX CAD Open API

# FormlimitsLeaderSetOutline - метод  
    
Установка параметров привязки к отрезку

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetOutline(
	Outline line,
	bool isOnEnd,
	Parameter offset
)
```




#### Параметры

line [Outline](T_TFlex_Model_Model2D_Outline.md)
    Отрезок привязки
isOnEnd [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Значение true указывает, что привязка выполняется к концу отрезка, false - к началу
offset [Parameter](T_TFlex_Model_Parameter.md)
    Смещение точки привязки по отрезку относительно выбранного конца отрезка

#### Ссылки

[FormlimitsLeader - ](T_TFlex_Model_Model2D_FormlimitsLeader.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)