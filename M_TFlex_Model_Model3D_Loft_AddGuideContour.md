

Руководство по T-FLEX CAD Open API

# LoftAddGuideContour - метод  
  
---  
  
Добавить контур к направляющей

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddGuideContour(
	int guideIndex,
	ModelContour contour
)
```
```vb
Public Sub AddGuideContour ( 
	guideIndex As Integer,
	contour As ModelContour
)
```
```cpp
public:
void AddGuideContour(
	int guideIndex, 
	ModelContour^ contour
)
```


#### Параметры

guideIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер направляющей (начинается с 0)
contour [ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)
    Добавляемый контур

Все контуры направляющей в списке одного типа: все листовые или все проволочные

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)