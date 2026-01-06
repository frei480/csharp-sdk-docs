

Руководство по T-FLEX CAD Open API

# BooleanGenerator - конструктор  
    
Конструктор для задания вытлакивания по направлению на заданные длины в прямом и обратном направлении

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public BooleanGenerator(
	ProxyObject3D object,
	Body target,
	Body[] tools,
	BooleanOperationFunctionType function
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	target As Body,
	tools As Body(),
	function As BooleanOperationFunctionType
)
```
```cpp
public:
BooleanGenerator(
	ProxyObject3D^ object, 
	Body^ target, 
	array<Body^>^ tools, 
	BooleanOperationFunctionType function
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
target [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Тело, к котому применятся булева
tools [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Массив тел, которые используются для модификации тела
function [BooleanOperationFunctionType](T_TFlex_Model_Model3D_BooleanOperation_FunctionType.md)
    Тип булевой

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[BooleanGenerator - ](T_TFlex_Model_Model3D_Geometry_BooleanGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)