

Руководство по T-FLEX CAD Open API

# LoftAddProfileFaceCondition - метод  
    
Добавить условие касания с гранью

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddProfileFaceCondition(
	int profileIndex,
	LoftFaceCondition condition
)
```




#### Параметры

profileIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс профиля (начинается нуля)
condition [LoftFaceCondition](T_TFlex_Model_Model3D_Loft_FaceCondition.md)
    Граничное условие

Грани должны стыковаться к профилю. Условия в виде граней не могут быть заданы, если для данного профиля задан другой тип граничного условия.

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)