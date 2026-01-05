

Руководство по T-FLEX CAD Open API

# BoxManipulatorBaseReset - метод  
  
---  
  
Устанавливает параметры настраиваемого параллелепипеда

**Пространство имён:** [TFlex.Model.Model3D.Visual.Manipulators](N_TFlex_Model_Model3D_Visual_Manipulators.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Reset(
	BasePoint3D origin,
	BaseDirection xDirection,
	BaseDirection yDirection,
	BaseDirection zDirection,
	double offsetX,
	double offsetY,
	double offsetZ
)
```
```vb
Public Sub Reset ( 
	origin As BasePoint3D,
	xDirection As BaseDirection,
	yDirection As BaseDirection,
	zDirection As BaseDirection,
	offsetX As Double,
	offsetY As Double,
	offsetZ As Double
)
```
```cpp
public:
void Reset(
	BasePoint3D^ origin, 
	BaseDirection^ xDirection, 
	BaseDirection^ yDirection, 
	BaseDirection^ zDirection, 
	double offsetX, 
	double offsetY, 
	double offsetZ
)
```


#### Параметры

origin [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    координаты одной из вершин параллелепипеда
xDirection [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    направление локальной оси X
yDirection [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    направление локальной оси Y
zDirection [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    направление локальной оси Z
offsetX [Double](https://learn.microsoft.com/dotnet/api/system.double)
    размер параллелепипеда вдоль локальной оси Z
offsetY [Double](https://learn.microsoft.com/dotnet/api/system.double)
    размер параллелепипеда вдоль локальной оси Z
offsetZ [Double](https://learn.microsoft.com/dotnet/api/system.double)
    размер параллелепипеда вдоль локальной оси Z

#### Ссылки

[BoxManipulatorBase - ](T_TFlex_Model_Model3D_Visual_Manipulators_BoxManipulatorBase.md)

[TFlex.Model.Model3D.Visual.Manipulators - пространство имён](N_TFlex_Model_Model3D_Visual_Manipulators.md)