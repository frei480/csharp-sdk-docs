

Руководство по T-FLEX CAD Open API

# LinearDimensionSetOutlineAndNode - метод  
    
Установка параметров размера между линией изображения и узлом

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetOutlineAndNode(
	Outline line1,
	bool isOnEnd1,
	Node node2
)
```




#### Параметры

line1 [Outline](T_TFlex_Model_Model2D_Outline.md)
    Отрезок
isOnEnd1 [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает на то, что размер прикреплен к концу отрезка (иначе - к началу)
node2 [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, до которого измеряется расстояние

#### Ссылки

[LinearDimension - ](T_TFlex_Model_Model2D_LinearDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)