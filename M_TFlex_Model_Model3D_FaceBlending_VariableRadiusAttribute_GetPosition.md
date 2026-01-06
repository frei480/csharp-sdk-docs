

Руководство по T-FLEX CAD Open API

# FaceBlendingVariableRadiusAttributeGetPosition - метод  
    
Удалить позицию

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FaceBlendingPositionData GetPosition(
	int positionIndex
)
```
```vb
Public Function GetPosition ( 
	positionIndex As Integer
) As FaceBlendingPositionData
```
```cpp
public:
FaceBlendingPositionData^ GetPosition(
	int positionIndex
)
```


#### Параметры

positionIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер позиции, должен быть в диапазоне 1..последняя позиция-1

#### Возвращаемое значение

[FaceBlendingPositionData](T_TFlex_Model_Model3D_FaceBlending_PositionData.md)Новый номер позиции

#### Ссылки

[FaceBlendingVariableRadiusAttribute - ](T_TFlex_Model_Model3D_FaceBlending_VariableRadiusAttribute.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)