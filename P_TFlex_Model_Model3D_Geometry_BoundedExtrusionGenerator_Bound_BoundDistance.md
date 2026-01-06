

Руководство по T-FLEX CAD Open API

# BoundedExtrusionGeneratorBoundBoundDistance - свойство  
    
Значение отступа

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public double BoundDistance { get; set; }
```
```vb
Public Property BoundDistance As Double
	Get
	Set
```
```cpp
public:
property double BoundDistance {
	double get ();
	void set (double value);
}
```


#### Значение свойства

[Double](https://learn.microsoft.com/dotnet/api/system.double)

Граница может задаваться четырьмя взаимоисключающими способами : листовым или твёрдым телом, гранью, поверхностью, отступом. Значение отступа можно задавать если выбран тип границы Distance.

#### Ссылки

[BoundedExtrusionGeneratorBound - ](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)