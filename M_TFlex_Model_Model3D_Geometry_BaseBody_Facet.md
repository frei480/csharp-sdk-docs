

Руководство по T-FLEX CAD Open API

# BaseBodyFacet - метод  
    
Функция создаёт плоскогранную сетку

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FacetMesh Facet(
	double tolerance,
	bool simplify,
	bool normal
)
```
```vb
Public Function Facet ( 
	tolerance As Double,
	simplify As Boolean,
	normal As Boolean
) As FacetMesh
```
```cpp
public:
FacetMesh^ Facet(
	double tolerance, 
	bool simplify, 
	bool normal
)
```


#### Параметры

tolerance [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
simplify [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
normal [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[FacetMesh](T_TFlex_Model_Model3D_Geometry_FacetMesh.md)Сетка

#### Ссылки

[BaseBody - ](T_TFlex_Model_Model3D_Geometry_BaseBody.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)