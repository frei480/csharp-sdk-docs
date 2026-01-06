

Руководство по T-FLEX CAD Open API

# LoftRemoveGuideContour - метод  
    
Удалить контур направляющей

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void RemoveGuideContour(
	int guideIndex,
	int contourIndex
)
```
```vb
Public Sub RemoveGuideContour ( 
	guideIndex As Integer,
	contourIndex As Integer
)
```
```cpp
public:
void RemoveGuideContour(
	int guideIndex, 
	int contourIndex
)
```


#### Параметры

guideIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер направляющей (начинается с 0)
contourIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер удаляемого контура (начинается с 0)

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)