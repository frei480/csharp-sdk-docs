

Руководство по T-FLEX CAD Open API

# ExtrudeGenerator - конструктор  
  
---  
  
Конструктор для задания выталкивания по направлению на заданные длины в прямом и обратном направлении

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ExtrudeGenerator(
	ProxyObject3D object,
	BaseDirection vector,
	Body profile,
	double length,
	double backLength
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	vector As BaseDirection,
	profile As Body,
	length As Double,
	backLength As Double
)
```
```cpp
public:
ExtrudeGenerator(
	ProxyObject3D^ object, 
	BaseDirection^ vector, 
	Body^ profile, 
	double length, 
	double backLength
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
vector [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Вектор направления выталкивания
profile [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Выталкиваемый контур. Этот контур превращается в выталкивание и возращается в списке результирующих тел или удаляется
length [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Величина длины выталкивания в прямом направлении
backLength [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Величина длины выталкивания в обратном направлении

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[ExtrudeGenerator - ](T_TFlex_Model_Model3D_Geometry_ExtrudeGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)