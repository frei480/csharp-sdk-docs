

Руководство по T-FLEX CAD Open API

# BoundedExtrusionGenerator - конструктор  
    
Конструктор для задания выталкивания от границы до границы

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public BoundedExtrusionGenerator(
	ProxyObject3D object,
	BaseDirection vector,
	Body profile,
	BoundedExtrusionGeneratorBound start,
	BoundedExtrusionGeneratorBound end
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	vector As BaseDirection,
	profile As Body,
	start As BoundedExtrusionGeneratorBound,
	end As BoundedExtrusionGeneratorBound
)
```
```cpp
public:
BoundedExtrusionGenerator(
	ProxyObject3D^ object, 
	BaseDirection^ vector, 
	Body^ profile, 
	BoundedExtrusionGeneratorBound^ start, 
	BoundedExtrusionGeneratorBound^ end
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
vector [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Вектор направления выталкивания
profile [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Выталкиваемый контур. Этот контур превращается в выталкивание и возращается в списке резльтирующих тел или удаляется
start [BoundedExtrusionGeneratorBound](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound.md)
    Первая граница выталкивания
end [BoundedExtrusionGeneratorBound](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound.md)
    Вторая граница выталкивания

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом.

#### Ссылки

[BoundedExtrusionGenerator - ](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)