

Руководство по T-FLEX CAD Open API

# FaceBlendingVariableRadiusAttributeSetPosition - метод  
    
Удалить позицию

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public int SetPosition(
	int positionIndex,
	FaceBlendingPositionData data
)
```
```vb
Public Function SetPosition ( 
	positionIndex As Integer,
	data As FaceBlendingPositionData
) As Integer
```
```cpp
public:
int SetPosition(
	int positionIndex, 
	FaceBlendingPositionData^ data
)
```


#### Параметры

positionIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер позиции, должен быть в диапазоне 1..последняя позиция-1
data [FaceBlendingPositionData](T_TFlex_Model_Model3D_FaceBlending_PositionData.md)
    Параметры заданные в позиции

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)Новый номер позиции

#### Ссылки

[FaceBlendingVariableRadiusAttribute - ](T_TFlex_Model_Model3D_FaceBlending_VariableRadiusAttribute.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)