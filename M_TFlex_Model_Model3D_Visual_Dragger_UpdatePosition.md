

Руководство по T-FLEX CAD Open API

# DraggerUpdatePosition - метод  
    
Обновление положения

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract bool UpdatePosition(
	View3D view,
	int x,
	int y
)
```
```vb
Public MustOverride Function UpdatePosition ( 
	view As View3D,
	x As Integer,
	y As Integer
) As Boolean
```
```cpp
public:
virtual bool UpdatePosition(
	View3D^ view, 
	int x, 
	int y
) abstract
```


#### Параметры

view [View3D](T_TFlex_Model_Model3D_View3D.md)
    Активный 3D вид
x [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Экранная координата X курсора
y [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Экранная координата Y курсора

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Должен возвращать true в случае, когда перемещение вызвало изменение данных и/или необходимость перерисовать декорации

Метод вызывается, когда пользователь перемещает мышь с зажатой левой кнопкой при активном манипуляторе

#### Ссылки

[Dragger - ](T_TFlex_Model_Model3D_Visual_Dragger.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)