

Руководство по T-FLEX CAD Open API

# OffsetSurfGetOffsetFace - метод  
  
---  
  
Получить особую грань

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void GetOffsetFace(
	int faceIndex,
	ref ModelFace face,
	ref Parameter offset
)
```
```vb
Public Sub GetOffsetFace ( 
	faceIndex As Integer,
	ByRef face As ModelFace,
	ByRef offset As Parameter
)
```
```cpp
public:
void GetOffsetFace(
	int faceIndex, 
	ModelFace^% face, 
	Parameter^% offset
)
```


#### Параметры

faceIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер грани
face [ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)
    Грань
offset [Parameter](T_TFlex_Model_Parameter.md)
    Смещение особой грани

#### Ссылки

[OffsetSurf - ](T_TFlex_Model_Model3D_OffsetSurf.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)