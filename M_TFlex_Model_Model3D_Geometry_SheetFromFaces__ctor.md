

Руководство по T-FLEX CAD Open API

# SheetFromFaces - конструктор  
    
Конструктор для задания листового тела по набору граней

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SheetFromFaces(
	ProxyObject3D object,
	BaseFace[] faces
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	faces As BaseFace()
)
```
```cpp
public:
SheetFromFaces(
	ProxyObject3D^ object, 
	array<BaseFace^>^ faces
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
faces [BaseFace](T_TFlex_Model_Model3D_Geometry_BaseFace.md)
    Множество граней

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[SheetFromFaces - ](T_TFlex_Model_Model3D_Geometry_SheetFromFaces.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)