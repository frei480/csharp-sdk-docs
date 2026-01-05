

Руководство по T-FLEX CAD Open API

# FaceFindAxis - метод  
  
---  
**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static bool FindAxis(
	IEnumerable<BaseTopol> faces,
	IEnumerable<BaseTopol> excludeEdges,
	ref BasePoint3D first,
	ref BasePoint3D second,
	byte useChainAlgorithm
)
```
```vb
Public Shared Function FindAxis ( 
	faces As IEnumerable(Of BaseTopol),
	excludeEdges As IEnumerable(Of BaseTopol),
	ByRef first As BasePoint3D,
	ByRef second As BasePoint3D,
	useChainAlgorithm As Byte
) As Boolean
```
```cpp
public:
static bool FindAxis(
	IEnumerable<BaseTopol^>^ faces, 
	IEnumerable<BaseTopol^>^ excludeEdges, 
	BasePoint3D^% first, 
	BasePoint3D^% second, 
	unsigned char useChainAlgorithm
)
```


#### Параметры

faces [IEnumerable](https://learn.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1)[BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)
    
excludeEdges [IEnumerable](https://learn.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1)[BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)
    
first [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    
second [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    
useChainAlgorithm [Byte](https://learn.microsoft.com/dotnet/api/system.byte)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[Face - ](T_TFlex_Model_Model3D_Geometry_Face.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)