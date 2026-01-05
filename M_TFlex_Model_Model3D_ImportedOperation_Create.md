

Руководство по T-FLEX CAD Open API

# ImportedOperationCreate(Document, ListBaseCurve, ListBaseInterval, ListPoint) - метод  
  
---  
**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static ImportedOperation Create(
	Document document,
	List<BaseCurve> curves,
	List<BaseInterval> intervals,
	List<Point> points
)
```
```vb
Public Shared Function Create ( 
	document As Document,
	curves As List(Of BaseCurve),
	intervals As List(Of BaseInterval),
	points As List(Of Point)
) As ImportedOperation
```
```cpp
public:
static ImportedOperation^ Create(
	Document^ document, 
	List<BaseCurve^>^ curves, 
	List<BaseInterval^>^ intervals, 
	List<Point>^ points
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    
curves [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)
    
intervals [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[BaseInterval](T_TFlex_Model_Model3D_Geometry_BaseInterval.md)
    
points [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[Point](T_TFlex_Drawing_Point.md)
    

#### Возвращаемое значение

[ImportedOperation](T_TFlex_Model_Model3D_ImportedOperation.md)

#### Ссылки

[ImportedOperation - ](T_TFlex_Model_Model3D_ImportedOperation.md)

[Create - перегрузка](Overload_TFlex_Model_Model3D_ImportedOperation_Create.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)