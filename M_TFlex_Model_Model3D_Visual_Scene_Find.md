

Руководство по T-FLEX CAD Open API

# SceneFind - метод  
    
Поиск узла, соответствующего данному объекту

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ObjectRepresentation Find(
	Object3D object
)
```
```vb
Public Function Find ( 
	object As Object3D
) As ObjectRepresentation
```
```cpp
public:
ObjectRepresentation^ Find(
	Object3D^ object
)
```


#### Параметры

object [Object3D](T_TFlex_Model_Model3D_Object3D.md)
    

#### Возвращаемое значение

[ObjectRepresentation](T_TFlex_Model_Model3D_Visual_ObjectRepresentation.md)

Возвращает null в случае, если объект не представлен в сцене

#### Ссылки

[Scene - ](T_TFlex_Model_Model3D_Visual_Scene.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)