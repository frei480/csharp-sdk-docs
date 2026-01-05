

Руководство по T-FLEX CAD Open API

# BoundedExtrusionBoundIntersection - свойство  
  
---  
  
Номер пересечения

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public int Intersection { set; }
```
```vb
Public WriteOnly Property Intersection As Integer
	Set
```
```cpp
public:
property int Intersection {
	void set (int value);
}
```


#### Значение свойства

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

Если граница имеет несколько пересечений с телом выталкивания, то можно явно задать номер сечения по направлению выталкивания. Передаваемый номер выталкивания используется для привязки изменяющегося в параметрической модели номера сечения в границе. В параметрической модели номер выталкивания может меняться. Поэтому его значения нельзя получить. Для направления, противоположного направлению выталкивания, номер задаётся отрицательным числом.

#### Ссылки

[BoundedExtrusionBound - ](T_TFlex_Model_Model3D_BoundedExtrusion_Bound.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)