

Руководство по T-FLEX CAD Open API

# CableCreateConductor - метод  
  
---  
**Пространство имён:** [TFlex.Model.Model3D.ConductorModel](N_TFlex_Model_Model3D_ConductorModel.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Conductor CreateConductor(
	MaterialParameter material,
	MaterialParameter coatingMaterial,
	Parameter color,
	Guid key
)
```
```vb
Public Function CreateConductor ( 
	material As MaterialParameter,
	coatingMaterial As MaterialParameter,
	color As Parameter,
	key As Guid
) As Conductor
```
```cpp
public:
Conductor^ CreateConductor(
	MaterialParameter^ material, 
	MaterialParameter^ coatingMaterial, 
	Parameter^ color, 
	Guid key
)
```


#### Параметры

material [MaterialParameter](T_TFlex_Model_Model3D_MaterialParameter.md)
    
coatingMaterial [MaterialParameter](T_TFlex_Model_Model3D_MaterialParameter.md)
    
color [Parameter](T_TFlex_Model_Parameter.md)
    
key [Guid](https://learn.microsoft.com/dotnet/api/system.guid)
    

#### Возвращаемое значение

[Conductor](T_TFlex_Model_Model3D_ConductorModel_Conductor.md)

#### Ссылки

[Cable - ](T_TFlex_Model_Model3D_ConductorModel_Cable.md)

[TFlex.Model.Model3D.ConductorModel - пространство имён](N_TFlex_Model_Model3D_ConductorModel.md)