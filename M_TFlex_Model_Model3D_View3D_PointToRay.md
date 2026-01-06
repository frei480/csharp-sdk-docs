

Руководство по T-FLEX CAD Open API

# View3DPointToRay - метод  
    
Преобразует точку на экране в луч в координатах модели

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool PointToRay(
	int x,
	int y,
	ref FloatVector rayStart,
	ref FloatVector rayDir
)
```




#### Параметры

x [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Абцисса точки на экране
y [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Ордината точки на экране
rayStart [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Исходная точка луча
rayDir [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Направление луча

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[View3D - ](T_TFlex_Model_Model3D_View3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)