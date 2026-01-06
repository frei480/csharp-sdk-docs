

Руководство по T-FLEX CAD Open API

# ConstructionOutline(Document, Node, Node, Construction) - конструктор  
    
Конструктор, задающий узлы, между которыми пройдет линия, и линию построения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ConstructionOutline(
	Document document,
	Node startNode,
	Node endNode,
	Construction srcConstruction
)
```




#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ объекта
startNode [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел
endNode [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел
srcConstruction [Construction](T_TFlex_Model_Model2D_Construction.md)
    Линия построения

При отсутствии линии построения будет создан отрезок между узлами

#### Ссылки

[ConstructionOutline - ](T_TFlex_Model_Model2D_ConstructionOutline.md)

[ConstructionOutline - перегрузка](Overload_TFlex_Model_Model2D_ConstructionOutline__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)