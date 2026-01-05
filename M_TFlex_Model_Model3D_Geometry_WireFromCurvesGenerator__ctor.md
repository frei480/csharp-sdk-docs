

Руководство по T-FLEX CAD Open API

# WireFromCurvesGenerator - конструктор  
  
---  
  
Конструктор для задания проволочного тела по набору кривых

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public WireFromCurvesGenerator(
	ProxyObject3D object,
	WireFromCurvesGeneratorSegment[] segments
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	segments As WireFromCurvesGeneratorSegment()
)
```
```cpp
public:
WireFromCurvesGenerator(
	ProxyObject3D^ object, 
	array<WireFromCurvesGeneratorSegment^>^ segments
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
segments [WireFromCurvesGeneratorSegment](T_TFlex_Model_Model3D_Geometry_WireFromCurvesGenerator_Segment.md)
    Множество сегментов

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[WireFromCurvesGenerator - ](T_TFlex_Model_Model3D_Geometry_WireFromCurvesGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)