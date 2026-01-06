

Руководство по T-FLEX CAD Open API

# SurfaceSplineDataRational - свойство  
    
Признак рациональности сплайна

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool Rational { get; set; }
```
```vb
Public Property Rational As Boolean
	Get
	Set
```
```cpp
public:
property bool Rational {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

При изменении типа на нерациональный информация о весах теряется. При изменении типа на рациональный все веса равны 1.0. Если тип не меняется, то информация о весах также не меняется

#### Ссылки

[SurfaceSplineData - ](T_TFlex_Model_Model3D_Geometry_SurfaceSplineData.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)