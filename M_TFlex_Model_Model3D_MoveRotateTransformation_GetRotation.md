

Руководство по T-FLEX CAD Open API

# MoveRotateTransformationGetRotation - метод  
    
Получить параметры поворота по индексу

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void GetRotation(
	int index,
	ref StandardAxis axisIndex,
	ref Parameter param
)
```




#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер поворота
axisIndex [StandardAxis](T_TFlex_Model_Model3D_StandardAxis.md)
    Если функция сработала успешно, то в неё помещается ось относительно которой производится поворот
param [Parameter](T_TFlex_Model_Parameter.md)
    Если функция сработала успешно, то в неё помещается значение угла поворота

#### Ссылки

[MoveRotateTransformation - ](T_TFlex_Model_Model3D_MoveRotateTransformation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)