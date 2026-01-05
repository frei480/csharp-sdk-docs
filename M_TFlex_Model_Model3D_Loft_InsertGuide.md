

Руководство по T-FLEX CAD Open API

# LoftInsertGuide - метод  
  
---  
  
Вставить направляющую в список направляющих

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void InsertGuide(
	int guideIndex,
	ModelContour contour
)
```
```vb
Public Sub InsertGuide ( 
	guideIndex As Integer,
	contour As ModelContour
)
```
```cpp
public:
void InsertGuide(
	int guideIndex, 
	ModelContour^ contour
)
```


#### Параметры

guideIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер добавляемой направляющей (начинается с 0)
contour [ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)
    

После добавления направляющей её нужно наполнить контурами с помощью функции AddGuideContour

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

[RemoveGuide(Int32)](M_TFlex_Model_Model3D_Loft_RemoveGuide.md)