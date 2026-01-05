

Руководство по T-FLEX CAD Open API

# ObjectNode(Document, UInt32, ModelObject) - конструктор  
  
---  
  
Конструктор, задающий родительский 3D объект и идентификатор узла

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ObjectNode(
	Document document,
	uint index,
	ModelObject parentObject
)
```
```vb
Public Sub New ( 
	document As Document,
	index As UInteger,
	parentObject As ModelObject
)
```
```cpp
public:
ObjectNode(
	Document^ document, 
	unsigned int index, 
	ModelObject^ parentObject
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ объекта
index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Идентификатор
parentObject [ModelObject](T_TFlex_Model_ModelObject.md)
    Родительский 3D объект

#### Ссылки

[ObjectNode - ](T_TFlex_Model_Model2D_ObjectNode.md)

[ObjectNode - перегрузка](Overload_TFlex_Model_Model2D_ObjectNode__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)