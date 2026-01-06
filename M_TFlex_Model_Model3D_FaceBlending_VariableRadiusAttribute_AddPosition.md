

Руководство по T-FLEX CAD Open API

# FaceBlendingVariableRadiusAttributeAddPosition - метод  
    
Добавить позицию

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public int AddPosition(
	FaceBlendingPositionData data
)
```
```vb
Public Function AddPosition ( 
	data As FaceBlendingPositionData
) As Integer
```
```cpp
public:
int AddPosition(
	FaceBlendingPositionData^ data
)
```


#### Параметры

data [FaceBlendingPositionData](T_TFlex_Model_Model3D_FaceBlending_PositionData.md)
    Параметры заданные в позиции

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)Номер добавленной позиции

Всегда существуют две позиции со значениями 0 и 100. Позиции всегда располагаются в порядке возрастания значения, добавление новых позиций может привести к изменению порядкового индекса ранее добавленных позиций

#### Ссылки

[FaceBlendingVariableRadiusAttribute - ](T_TFlex_Model_Model3D_FaceBlending_VariableRadiusAttribute.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)