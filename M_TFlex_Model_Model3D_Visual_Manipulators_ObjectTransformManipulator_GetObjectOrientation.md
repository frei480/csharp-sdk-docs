

Руководство по T-FLEX CAD Open API

# ObjectTransformManipulatorGetObjectOrientation - метод  
  **Пространство имён:** [TFlex.Model.Model3D.Visual.Manipulators](N_TFlex_Model_Model3D_Visual_Manipulators.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static bool GetObjectOrientation(
	Object3D object,
	ref Point3D origin,
	ref Direction dirX,
	ref Direction dirY,
	ref Direction dirZ
)
```
```vb
Public Shared Function GetObjectOrientation ( 
	object As Object3D,
	ByRef origin As Point3D,
	ByRef dirX As Direction,
	ByRef dirY As Direction,
	ByRef dirZ As Direction
) As Boolean
```
```cpp
public:
static bool GetObjectOrientation(
	Object3D^ object, 
	Point3D^% origin, 
	Direction^% dirX, 
	Direction^% dirY, 
	Direction^% dirZ
)
```


#### Параметры

object [Object3D](T_TFlex_Model_Model3D_Object3D.md)
    
origin [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    
dirX [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
dirY [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
dirZ [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[ObjectTransformManipulator - ](T_TFlex_Model_Model3D_Visual_Manipulators_ObjectTransformManipulator.md)

[TFlex.Model.Model3D.Visual.Manipulators - пространство имён](N_TFlex_Model_Model3D_Visual_Manipulators.md)