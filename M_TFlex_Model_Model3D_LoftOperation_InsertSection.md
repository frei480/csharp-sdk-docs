

Руководство по T-FLEX CAD Open API

# LoftOperationInsertSection - метод  
    
Вставить сечение

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public LoftOperationSection InsertSection(
	int sectionIndex,
	ModelContour contour
)
```
```vb
Public Function InsertSection ( 
	sectionIndex As Integer,
	contour As ModelContour
) As LoftOperationSection
```
```cpp
public:
LoftOperationSection^ InsertSection(
	int sectionIndex, 
	ModelContour^ contour
)
```


#### Параметры

sectionIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс добавляемого сечения (начинается с 0)
contour [ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)
    

#### Возвращаемое значение

[LoftOperationSection](T_TFlex_Model_Model3D_LoftOperation_Section.md)

#### Ссылки

[LoftOperation - ](T_TFlex_Model_Model3D_LoftOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)