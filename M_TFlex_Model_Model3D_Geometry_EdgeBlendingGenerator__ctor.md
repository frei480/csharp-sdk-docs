

Руководство по T-FLEX CAD Open API

# EdgeBlendingGenerator - конструктор  
  
---  
  
Конструктор для задания базовых объектов сглаживания

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public EdgeBlendingGenerator(
	ProxyObject3D object,
	Body body
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	body As Body
)
```
```cpp
public:
EdgeBlendingGenerator(
	ProxyObject3D^ object, 
	Body^ body
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
body [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Тело на котором строится сглаживание

3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[EdgeBlendingGenerator - ](T_TFlex_Model_Model3D_Geometry_EdgeBlendingGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)