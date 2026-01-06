

Руководство по T-FLEX CAD Open API

# OutlinesIntersection - конструктор  
    
Конструктор

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public OutlinesIntersection(
	Document document,
	Outline outline1,
	Outline outline2,
	int point,
	OutlinesIntersectionForms form,
	Parameter size,
	Parameter lineWidth
)
```
```vb
Public Sub New ( 
	document As Document,
	outline1 As Outline,
	outline2 As Outline,
	point As Integer,
	form As OutlinesIntersectionForms,
	size As Parameter,
	lineWidth As Parameter
)
```
```cpp
public:
OutlinesIntersection(
	Document^ document, 
	Outline^ outline1, 
	Outline^ outline2, 
	int point, 
	OutlinesIntersectionForms form, 
	Parameter^ size, 
	Parameter^ lineWidth
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ
outline1 [Outline](T_TFlex_Model_Model2D_Outline.md)
    Первая линия изображения
outline2 [Outline](T_TFlex_Model_Model2D_Outline.md)
    Вторая линия изображения
point [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки пересечения
form [OutlinesIntersectionForms](T_TFlex_Model_Model2D_OutlinesIntersection_Forms.md)
    Форма обозначения
size [Parameter](T_TFlex_Model_Parameter.md)
    Размер обозначения
lineWidth [Parameter](T_TFlex_Model_Parameter.md)
    Толлщина линии обозначения

#### Ссылки

[OutlinesIntersection - ](T_TFlex_Model_Model2D_OutlinesIntersection.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)