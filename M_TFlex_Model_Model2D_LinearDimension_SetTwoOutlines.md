

Руководство по T-FLEX CAD Open API

# LinearDimensionSetTwoOutlines - метод  
    
Установка параметров размера между двумя линиями изображения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTwoOutlines(
	Outline line1,
	bool isOnEnd1,
	Outline line2,
	bool isOnEnd2,
	bool isConusDim
)
```




#### Параметры

line1 [Outline](T_TFlex_Model_Model2D_Outline.md)
    Первый отрезок
isOnEnd1 [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает на то, что размер прикреплен к концу отрезка (иначе - к началу)
line2 [Outline](T_TFlex_Model_Model2D_Outline.md)
    Второй отрезок
isOnEnd2 [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает на то, что размер прикреплен к концу отрезка (иначе - к началу)
isConusDim [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Параметр, показывающий что размер ставится на конусе, ребрами которого являются отрезки, иначе - размер берётся как расстояние между отрезками

#### Ссылки

[LinearDimension - ](T_TFlex_Model_Model2D_LinearDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)