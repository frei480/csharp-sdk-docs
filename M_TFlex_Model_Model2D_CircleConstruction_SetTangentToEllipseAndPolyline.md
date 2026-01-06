

Руководство по T-FLEX CAD Open API

# CircleConstructionSetTangentToEllipseAndPolyline - метод  
    
Окружность, касательная к эллипсу и сплайну или другой полилинии

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTangentToEllipseAndPolyline(
	Construction srcEllipse,
	Construction srcPolyline,
	Parameter radius,
	int variant
)
```




#### Параметры

srcEllipse [Construction](T_TFlex_Model_Model2D_Construction.md)
    Эллипс, которого касается окружность
srcPolyline [Construction](T_TFlex_Model_Model2D_Construction.md)
    Полилиния, которой касается окружность
radius [Parameter](T_TFlex_Model_Parameter.md)
    Радиус окружности
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер варианта касания

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)