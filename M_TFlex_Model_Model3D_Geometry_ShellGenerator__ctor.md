

Руководство по T-FLEX CAD Open API

# ShellGenerator - конструктор  
    
Конструктор для задания базовых объектов построения оболочки

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ShellGenerator(
	ProxyObject3D object,
	Body body,
	bool isEquid,
	double defDist
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	body As Body,
	isEquid As Boolean,
	defDist As Double
)
```
```cpp
public:
ShellGenerator(
	ProxyObject3D^ object, 
	Body^ body, 
	bool isEquid, 
	double defDist
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
body [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Тело на котором строится оболочка
isEquid [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Параметр режима построения оболочка или эквидистантное тело
defDist [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Толщина стенки по умолчанию в метрах

3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[ShellGenerator - ](T_TFlex_Model_Model3D_Geometry_ShellGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)