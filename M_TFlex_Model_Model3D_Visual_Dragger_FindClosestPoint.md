

Руководство по T-FLEX CAD Open API

# DraggerFindClosestPoint - метод  
    
Поиск ближайшей точки на декорациях

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
protected Decoration FindClosestPoint(
	View3D view,
	int x,
	int y,
	float tolerance,
	ref FloatVector closestPoint
)
```




#### Параметры

view [View3D](T_TFlex_Model_Model3D_View3D.md)
    Активный 3D вид
x [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Экранная координата X курсора
y [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Экранная координата Y курсора
tolerance [Single](https://learn.microsoft.com/dotnet/api/system.single)
    Допустимое расстояние от курсора до декорации
closestPoint [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Ближайшая найденная точка на декорации

#### Возвращаемое значение

[Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)Декорация, которой непосредственно принадлежит найденная точка, или 0 в случае ошибки

Этим методом рекомендуется пользоваться внутри перекрытого метода Activated для того, чтобы найти точку, в которой луч пересёк декорации. 

#### Ссылки

[Dragger - ](T_TFlex_Model_Model3D_Visual_Dragger.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)