

Руководство по T-FLEX CAD Open API

# LoftOperationInsertGuide - метод  
    
Вставить направляющую

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public LoftOperationGuide InsertGuide(
	int guideIndex,
	ModelContour contour
)
```
```vb
Public Function InsertGuide ( 
	guideIndex As Integer,
	contour As ModelContour
) As LoftOperationGuide
```
```cpp
public:
LoftOperationGuide^ InsertGuide(
	int guideIndex, 
	ModelContour^ contour
)
```


#### Параметры

guideIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс направляющей (начинается с 0)
contour [ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)
    

#### Возвращаемое значение

[LoftOperationGuide](T_TFlex_Model_Model3D_LoftOperation_Guide.md)

#### Ссылки

[LoftOperation - ](T_TFlex_Model_Model3D_LoftOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)