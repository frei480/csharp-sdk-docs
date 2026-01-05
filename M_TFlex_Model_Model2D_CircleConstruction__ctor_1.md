

Руководство по T-FLEX CAD Open API

# CircleConstruction(Document, Point, Construction, Construction) - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public CircleConstruction(
	Document document,
	Point centerPoint,
	Construction firstTangentPolyline,
	Construction secondTangentPolyline
)
```
```vb
Public Sub New ( 
	document As Document,
	centerPoint As Point,
	firstTangentPolyline As Construction,
	secondTangentPolyline As Construction
)
```
```cpp
public:
CircleConstruction(
	Document^ document, 
	Point centerPoint, 
	Construction^ firstTangentPolyline, 
	Construction^ secondTangentPolyline
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ, в котором создаётся новый объект
centerPoint [Point](T_TFlex_Drawing_Point.md)
    Точка задающая положение окружности
firstTangentPolyline [Construction](T_TFlex_Model_Model2D_Construction.md)
    Первый сплайн (полилиния), которого касается окружность
secondTangentPolyline [Construction](T_TFlex_Model_Model2D_Construction.md)
    Второй сплайн (полилиния), которого касается окружность

#### Ссылки

[CircleConstruction - ](T_TFlex_Model_Model2D_CircleConstruction.md)

[CircleConstruction - перегрузка](Overload_TFlex_Model_Model2D_CircleConstruction__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)