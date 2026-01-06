

Руководство по T-FLEX CAD Open API

# ConductorSetCreateCable - метод  
  **Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Cable CreateCable(
	MaterialParameter material,
	MaterialParameter coatingMaterial,
	Parameter color,
	Guid key
)
```
```vb
Public Function CreateCable ( 
	material As MaterialParameter,
	coatingMaterial As MaterialParameter,
	color As Parameter,
	key As Guid
) As Cable
```
```cpp
public:
Cable^ CreateCable(
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

[Cable](T_TFlex_Model_Model3D_ConductorModel_Cable.md)

#### Ссылки

[ConductorSet - ](T_TFlex_Model_Model3D_ConductorSet.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)