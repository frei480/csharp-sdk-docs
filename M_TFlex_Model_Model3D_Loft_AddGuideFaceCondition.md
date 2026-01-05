

Руководство по T-FLEX CAD Open API

# LoftAddGuideFaceCondition - метод  
  
---  
  
Добавить условие касания с гранью

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddGuideFaceCondition(
	int guideIndex,
	LoftFaceCondition condition
)
```
```vb
Public Sub AddGuideFaceCondition ( 
	guideIndex As Integer,
	condition As LoftFaceCondition
)
```
```cpp
public:
void AddGuideFaceCondition(
	int guideIndex, 
	LoftFaceCondition^ condition
)
```


#### Параметры

guideIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс направляющей (начинается с нуля)
condition [LoftFaceCondition](T_TFlex_Model_Model3D_Loft_FaceCondition.md)
    Граничное условие

Грани должны стыковаться c направляющей. Условия в виде граней не могут быть заданы, если для данной направляющей задан другой тип граничного условия.

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)