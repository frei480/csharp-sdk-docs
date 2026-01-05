

Руководство по T-FLEX CAD Open API

# EdgeBlendingAddEdgesByVertex - метод  
  
---  
  
Для всех рёбер, инцидентных данной вершине, задаются отступы

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public int AddEdgesByVertex(
	ModelVertex vertex,
	Parameter distance,
	bool common
)
```
```vb
Public Function AddEdgesByVertex ( 
	vertex As ModelVertex,
	distance As Parameter,
	common As Boolean
) As Integer
```
```cpp
public:
int AddEdgesByVertex(
	ModelVertex^ vertex, 
	Parameter^ distance, 
	bool common
)
```


#### Параметры

vertex [ModelVertex](T_TFlex_Model_Model3D_Geometry_ModelVertex.md)
    Вершина
distance [Parameter](T_TFlex_Model_Parameter.md)
    Значение отступа
common [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Параметр установлен для всех вершин

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

#### Ссылки

[EdgeBlending - ](T_TFlex_Model_Model3D_EdgeBlending.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)