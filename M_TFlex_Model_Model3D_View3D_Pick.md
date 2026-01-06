

Руководство по T-FLEX CAD Open API

# View3DPick - метод  
    
Ищет точку на декорации по заданным экранным координатам

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Decoration Pick(
	int x,
	int y,
	float tolerance,
	Decoration decorationRoot,
	ref FloatVector closestPoint
)
```
```vb
Public Function Pick ( 
	x As Integer,
	y As Integer,
	tolerance As Single,
	decorationRoot As Decoration,
	ByRef closestPoint As FloatVector
) As Decoration
```
```cpp
public:
Decoration^ Pick(
	int x, 
	int y, 
	float tolerance, 
	Decoration^ decorationRoot, 
	FloatVector% closestPoint
)
```


#### Параметры

x [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Экранная координата X
y [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Экранная координата Y
tolerance [Single](https://learn.microsoft.com/dotnet/api/system.single)
    Допустимое расстояние в пикселях от точки на экране до декорации
decorationRoot [Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)
    Декорация, на которой ведется поиск
closestPoint [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Найденная ближайшая точка на декорации

#### Возвращаемое значение

[Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)Декорация, которой непосредственно принадлежит найденная точка. Отличается от decorationRoot в случае, если decorationRoot - контейнер декораций. NULL в случае, если точка не найдена.

#### Ссылки

[View3D - ](T_TFlex_Model_Model3D_View3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)