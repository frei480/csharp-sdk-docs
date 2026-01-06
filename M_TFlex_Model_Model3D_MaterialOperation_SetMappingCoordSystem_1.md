

Руководство по T-FLEX CAD Open API

# MaterialOperationSetMappingCoordSystem(Int32, LCS) - метод  
    
Установить систему координат наложения текстуры для данной группы граней

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetMappingCoordSystem(
	int Group,
	LCS lcs
)
```
```vb
Public Sub SetMappingCoordSystem ( 
	Group As Integer,
	lcs As LCS
)
```
```cpp
public:
void SetMappingCoordSystem(
	int Group, 
	LCS^ lcs
)
```


#### Параметры

Group [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
lcs [LCS](T_TFlex_Model_Model3D_LCS.md)
    

Система координат определена для наложения проецированием на плоскость, цилиндр, сферу, параллелепипед

#### Ссылки

[MaterialOperation - ](T_TFlex_Model_Model3D_MaterialOperation.md)

[SetMappingCoordSystem - перегрузка](Overload_TFlex_Model_Model3D_MaterialOperation_SetMappingCoordSystem.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)