

Руководство по T-FLEX CAD Open API

# ConstructionOutline(Document, Construction) - конструктор  
    
Конструктор, задающий линию построения по которой будет построена новая линия. 

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ConstructionOutline(
	Document document,
	Construction srcConstruction
)
```
```vb
Public Sub New ( 
	document As Document,
	srcConstruction As Construction
)
```
```cpp
public:
ConstructionOutline(
	Document^ document, 
	Construction^ srcConstruction
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ объекта
srcConstruction [Construction](T_TFlex_Model_Model2D_Construction.md)
    Линия построения

В качестве линии построения не может быть задана прямая

#### Ссылки

[ConstructionOutline - ](T_TFlex_Model_Model2D_ConstructionOutline.md)

[ConstructionOutline - перегрузка](Overload_TFlex_Model_Model2D_ConstructionOutline__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)