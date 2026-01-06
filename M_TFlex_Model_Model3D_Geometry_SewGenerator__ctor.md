

Руководство по T-FLEX CAD Open API

# SewGenerator - конструктор  
    
Конструктор для задания сшивки

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SewGenerator(
	ProxyObject3D object,
	Body[] sheets,
	double gap
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	sheets As Body(),
	gap As Double
)
```
```cpp
public:
SewGenerator(
	ProxyObject3D^ object, 
	array<Body^>^ sheets, 
	double gap
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
sheets [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Множество сшиваемых листовых тел
gap [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Минимальное значение ширины щели

Все параметры обязятельные. 3D объект внешнего приложения должен быть связан с внешним объектом.

#### Ссылки

[SewGenerator - ](T_TFlex_Model_Model3D_Geometry_SewGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)