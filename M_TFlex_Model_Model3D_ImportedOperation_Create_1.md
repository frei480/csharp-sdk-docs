

Руководство по T-FLEX CAD Open API

# ImportedOperationCreate(Document, BasePoint3D, BasePoint3D, BasePoint3D) - метод  
  
---  
  
Конструктор для операции "Внешняя модель"

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static ImportedOperation Create(
	Document document,
	BasePoint3D point0,
	BasePoint3D point1,
	BasePoint3D point2
)
```
```vb
Public Shared Function Create ( 
	document As Document,
	point0 As BasePoint3D,
	point1 As BasePoint3D,
	point2 As BasePoint3D
) As ImportedOperation
```
```cpp
public:
static ImportedOperation^ Create(
	Document^ document, 
	BasePoint3D^ point0, 
	BasePoint3D^ point1, 
	BasePoint3D^ point2
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ, в котором создаётся новый объект
point0 [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    
point1 [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    
point2 [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    

#### Возвращаемое значение

[ImportedOperation](T_TFlex_Model_Model3D_ImportedOperation.md)

#### Ссылки

[ImportedOperation - ](T_TFlex_Model_Model3D_ImportedOperation.md)

[Create - перегрузка](Overload_TFlex_Model_Model3D_ImportedOperation_Create.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)