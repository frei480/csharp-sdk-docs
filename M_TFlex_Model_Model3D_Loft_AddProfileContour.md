

Руководство по T-FLEX CAD Open API

# LoftAddProfileContour - метод  
  
---  
  
Добавить контур к профилю

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddProfileContour(
	int profileIndex,
	ModelContour contour
)
```
```vb
Public Sub AddProfileContour ( 
	profileIndex As Integer,
	contour As ModelContour
)
```
```cpp
public:
void AddProfileContour(
	int profileIndex, 
	ModelContour^ contour
)
```


#### Параметры

profileIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер профиля (начинается с 0)
contour [ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)
    Добавляемый контур

Все контуры профиля в списке одного типа: все листовые или все проволочные

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)