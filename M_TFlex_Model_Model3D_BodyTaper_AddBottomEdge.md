

Руководство по T-FLEX CAD Open API

# BodyTaperAddBottomEdge - метод  
    
Добавить нижнее ребро

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddBottomEdge(
	ModelEdge edge,
	bool miter,
	bool replace,
	BodyTaperMethodType method
)
```
```vb
Public Sub AddBottomEdge ( 
	edge As ModelEdge,
	miter As Boolean,
	replace As Boolean,
	method As BodyTaperMethodType
)
```
```cpp
public:
void AddBottomEdge(
	ModelEdge^ edge, 
	bool miter, 
	bool replace, 
	BodyTaperMethodType method
)
```


#### Параметры

edge [ModelEdge](T_TFlex_Model_Model3D_Geometry_ModelEdge.md)
    
miter [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
replace [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
method [BodyTaperMethodType](T_TFlex_Model_Model3D_BodyTaper_MethodType.md)
    

#### Ссылки

[BodyTaper - ](T_TFlex_Model_Model3D_BodyTaper.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)