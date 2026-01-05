

Руководство по T-FLEX CAD Open API

# IntersectionNode(Document, Construction, Construction, Int32) - конструктор  
  
---  
  
Конструктор, задающий линии построения, на пересечении которых находится узел и вариант пересечения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public IntersectionNode(
	Document document,
	Construction srcConstruction1,
	Construction srcConstruction2,
	int variant
)
```
```vb
Public Sub New ( 
	document As Document,
	srcConstruction1 As Construction,
	srcConstruction2 As Construction,
	variant As Integer
)
```
```cpp
public:
IntersectionNode(
	Document^ document, 
	Construction^ srcConstruction1, 
	Construction^ srcConstruction2, 
	int variant
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ объекта
srcConstruction1 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первая линия построения
srcConstruction2 [Construction](T_TFlex_Model_Model2D_Construction.md)
    Вторая линия построения
variant [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Вариант исполнения

#### Ссылки

[IntersectionNode - ](T_TFlex_Model_Model2D_IntersectionNode.md)

[IntersectionNode - перегрузка](Overload_TFlex_Model_Model2D_IntersectionNode__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)