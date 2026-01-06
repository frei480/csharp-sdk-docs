

Руководство по T-FLEX CAD Open API

# EdgeBlendingAddTopol(ModelTopol, EdgeBlendingAttribute) - метод  
    
Добавить топологию со своими атрибутами

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddTopol(
	ModelTopol topol,
	EdgeBlendingAttribute attrib
)
```
```vb
Public Sub AddTopol ( 
	topol As ModelTopol,
	attrib As EdgeBlendingAttribute
)
```
```cpp
public:
void AddTopol(
	ModelTopol^ topol, 
	EdgeBlendingAttribute^ attrib
)
```


#### Параметры

topol [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)
    Топология
attrib [EdgeBlendingAttribute](T_TFlex_Model_Model3D_EdgeBlending_Attribute.md)
    

Топология должна быть ребром, циклом или гранью. Независимо от типа топологии, у топологии используются только рёбра. Гладкосопряженные рёбра должны быть определены с одинаковыми атрибутами, в противном случае результат не специфицирован

#### Ссылки

[EdgeBlending - ](T_TFlex_Model_Model3D_EdgeBlending.md)

[AddTopol - перегрузка](Overload_TFlex_Model_Model3D_EdgeBlending_AddTopol.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)