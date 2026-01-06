

Руководство по T-FLEX CAD Open API

# LoftGetGuideVectorCondition - метод  
    
Получить векторное условие на направляющей

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public LoftVectorCondition GetGuideVectorCondition(
	int guideIndex,
	int guideVectorConditionIndex
)
```
```vb
Public Function GetGuideVectorCondition ( 
	guideIndex As Integer,
	guideVectorConditionIndex As Integer
) As LoftVectorCondition
```
```cpp
public:
LoftVectorCondition^ GetGuideVectorCondition(
	int guideIndex, 
	int guideVectorConditionIndex
)
```


#### Параметры

guideIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс направляющей (начинается с нуля)
guideVectorConditionIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер векторного граничного условия

#### Возвращаемое значение

[LoftVectorCondition](T_TFlex_Model_Model3D_Loft_VectorCondition.md)

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)