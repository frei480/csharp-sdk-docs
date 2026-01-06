

Руководство по T-FLEX CAD Open API

# IntersectionNode(Document, Construction, Construction, Double, Double) - конструктор  
    
Конструктор, задающий линии построения, на пересечении которых находится узел и координаты точки, ближайшей к требуемому варианту пересечения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public IntersectionNode(
	Document document,
	Construction srcConstruction1,
	Construction srcConstruction2,
	double x,
	double y
)
```
```vb
Public Sub New ( 
	document As Document,
	srcConstruction1 As Construction,
	srcConstruction2 As Construction,
	x As Double,
	y As Double
)
```
```cpp
public:
IntersectionNode(
	Document^ document, 
	Construction^ srcConstruction1, 
	Construction^ srcConstruction2, 
	double x, 
	double y
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ объекта
srcConstruction1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая линия построения
srcConstruction2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая линия построения
x [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Коордианата X точки
y [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Коордианата Y точки

#### Ссылки

[IntersectionNode - ](T_TFlex_Model_Model2D_IntersectionNode.md)

[IntersectionNode - перегрузка](Overload_TFlex_Model_Model2D_IntersectionNode__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)