

Руководство по T-FLEX CAD Open API

# CenterAxisOutline(Document, Outline, CenterAxisOutlineCenterAxisType, Outline, Outline, Outline, Node, Node) - конструктор  
  
---  
  
Конструктор для создания оси от центра, заданного дугой или окружностью изображения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public CenterAxisOutline(
	Document document,
	Outline source,
	CenterAxisOutlineCenterAxisType axisType,
	Outline centerOutline,
	Outline limit1Outline,
	Outline limit2Outline,
	Node limit1Node,
	Node limit2Node
)
```
```vb
Public Sub New ( 
	document As Document,
	source As Outline,
	axisType As CenterAxisOutlineCenterAxisType,
	centerOutline As Outline,
	limit1Outline As Outline,
	limit2Outline As Outline,
	limit1Node As Node,
	limit2Node As Node
)
```
```cpp
public:
CenterAxisOutline(
	Document^ document, 
	Outline^ source, 
	CenterAxisOutlineCenterAxisType axisType, 
	Outline^ centerOutline, 
	Outline^ limit1Outline, 
	Outline^ limit2Outline, 
	Node^ limit1Node, 
	Node^ limit2Node
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ
source [Outline](T_TFlex_Model_Model2D_Outline.md)
    Обозначаемая линия изображения
axisType [CenterAxisOutlineCenterAxisType](T_TFlex_Model_Model2D_CenterAxisOutline_CenterAxisType.md)
    Тип оси
centerOutline [Outline](T_TFlex_Model_Model2D_Outline.md)
    Окружность или дуга, определяющая центр
limit1Outline [Outline](T_TFlex_Model_Model2D_Outline.md)
    Первая ограничивающая линия изображения (допускается значение null)
limit2Outline [Outline](T_TFlex_Model_Model2D_Outline.md)
    Вторая ограничивающая линия изображения (допускается значение null)
limit1Node [Node](T_TFlex_Model_Model2D_Node.md)
    Первый ограничивающий узел (допускается значение null)
limit2Node [Node](T_TFlex_Model_Model2D_Node.md)
    Второй ограничивающий узел (допускается значение null)

#### Ссылки

[CenterAxisOutline - ](T_TFlex_Model_Model2D_CenterAxisOutline.md)

[CenterAxisOutline - перегрузка](Overload_TFlex_Model_Model2D_CenterAxisOutline__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)