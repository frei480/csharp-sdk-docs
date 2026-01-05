

Руководство по T-FLEX CAD Open API

# SpatialWorkSurfaceBoundQuadrant - свойство  
  
---  
  
Квадрант границы рабочей поверхности, если границы задаются одним узлом и границами листа

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public int BoundQuadrant { get; set; }
```
```vb
Public Property BoundQuadrant As Integer
	Get
	Set
```
```cpp
public:
property int BoundQuadrant {
	int get ();
	void set (int value);
}
```


#### Значение свойства

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

Квадранты нумеруются от 1 до 4. По умолчанию первый угол задаётся точкой привязки

#### Ссылки

[SpatialWorkSurface - ](T_TFlex_Model_Model3D_SpatialWorkSurface.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)