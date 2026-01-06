

Руководство по T-FLEX CAD Open API

# SweepGenerator - конструктор  
    
Конструктор для задания тела по траектории

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SweepGenerator(
	ProxyObject3D object,
	Body profile,
	Body path,
	Vertex start
)
```




#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
profile [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Образующий контур. Этот контур превращается в тело по траектории и возращается в списке резльтирующих тел или удаляется
path [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Траектория
start [Vertex](T_TFlex_Model_Model3D_Geometry_Vertex.md)
    Стартовая точка на траектории

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[SweepGenerator - ](T_TFlex_Model_Model3D_Geometry_SweepGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)