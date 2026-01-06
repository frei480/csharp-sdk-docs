

Руководство по T-FLEX CAD Open API

# DraggerActivate - метод  
    
Активизация манипулятора

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract bool Activate(
	View3D view,
	int x,
	int y,
	float tolerance
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

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Должен возвращать true в случае, когда манипулятор может активизироваться, иначе false

Метод вызывается, когда пользователь нажал на кнопку мыши в тот момент, когда курсор находился над декорацией, ассоциированной с манипулятором. Для определения ближайшей к курсору точки на декорации можно воспользоваться методом FindClosestPoint со входными параметрами данного метода 

#### Ссылки

[Dragger - ](T_TFlex_Model_Model3D_Visual_Dragger.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)