

Руководство по T-FLEX CAD Open API

# LoftGetGuideFaceCondition - метод  
    
Получить условие касания с гранью

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public LoftFaceCondition GetGuideFaceCondition(
	int guideIndex,
	int guideFaceConditionIndex
)
```




#### Параметры

guideIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс направляющей (начинается с нуля)
guideFaceConditionIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс грани задающей каксательное условие

#### Возвращаемое значение

[LoftFaceCondition](T_TFlex_Model_Model3D_Loft_FaceCondition.md)Граничное условие

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)