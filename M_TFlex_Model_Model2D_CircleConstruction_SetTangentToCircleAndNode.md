

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTangentToCircleAndNode - метод  
    
Окружность, касательная к окружности, проходящая через узел

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToCircleAndNode(
	Construction srcCircle,
	Node srcNode,
	Parameter radius,
	int variant
)
```




#### Параметры

srcCircle [Construction](T_TFlex_Model_Model2D_Construction.md)
    Окружность, которой касается окружность
srcNode [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, через который проходит окружность
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус окружности
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)