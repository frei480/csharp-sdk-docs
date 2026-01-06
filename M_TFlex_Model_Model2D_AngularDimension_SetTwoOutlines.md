

Руководство по T-FLEX CAD Open API

# AngularDimensionSetTwoOutlines - метод  
    
Установка параметров размера между двумя линиями изображения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetTwoOutlines(
	Outline line1,
	bool isOnEnd1,
	Outline line2,
	bool isOnEnd2,
	AnglePosition position
)
```
```vb
Public Sub SetTwoOutlines ( 
	line1 As Outline,
	isOnEnd1 As Boolean,
	line2 As Outline,
	isOnEnd2 As Boolean,
	position As AnglePosition
)
```
```cpp
public:
void SetTwoOutlines(
	Outline^ line1, 
	bool isOnEnd1, 
	Outline^ line2, 
	bool isOnEnd2, 
	AnglePosition position
)
```


#### Параметры

line1 [Outline](T_TFlex_Model_Model2D_Outline.md)
    Первый отрезок
isOnEnd1 [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает на то, что размер прикреплен к концу отрезка (иначе - к началу)
line2 [Outline](T_TFlex_Model_Model2D_Outline.md)
    Второй отрезок
isOnEnd2 [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает на то, что размер прикреплен к концу отрезка (иначе - к началу)
position [AnglePosition](T_TFlex_Model_Model2D_AnglePosition.md)
    Между какими направлениями измеряется угол

#### Ссылки

[AngularDimension - ](T_TFlex_Model_Model2D_AngularDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)