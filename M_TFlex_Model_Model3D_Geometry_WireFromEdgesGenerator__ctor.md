

Руководство по T-FLEX CAD Open API

# WireFromEdgesGenerator - конструктор  
    
Конструктор для задания проволочного тела по набору рёбер с разных тел

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public WireFromEdgesGenerator(
	ProxyObject3D object,
	BaseEdge[] edges
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	edges As BaseEdge()
)
```
```cpp
public:
WireFromEdgesGenerator(
	ProxyObject3D^ object, 
	array<BaseEdge^>^ edges
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
edges [BaseEdge](T_TFlex_Model_Model3D_Geometry_BaseEdge.md)
    Множество рёбер

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[WireFromEdgesGenerator - ](T_TFlex_Model_Model3D_Geometry_WireFromEdgesGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)