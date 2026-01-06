

Руководство по T-FLEX CAD Open API

# EuclideanWorkplaneManagerMakeArray - метод  
    
Создать группу рабочих плоскостей

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static void MakeArray(
	Workplane plane1,
	Workplane plane2,
	int nCount,
	bool fUseStep,
	double step,
	double beginOffset,
	double endOffset
)
```




#### Параметры

plane1 [Workplane](T_TFlex_Model_Model3D_Workplane.md)
    Первая плоскость
plane2 [Workplane](T_TFlex_Model_Model3D_Workplane.md)
    Вторая плоскость
nCount [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
fUseStep [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    true - использовать значение шага step, иначе - определять шаг по расстоянию между данными плоскостями и количеству nCount
step [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
beginOffset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Начальное смещение
endOffset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Конечное смещение

#### Ссылки

[EuclideanWorkplaneManager - ](T_TFlex_Model_Model3D_EuclideanWorkplaneManager.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)