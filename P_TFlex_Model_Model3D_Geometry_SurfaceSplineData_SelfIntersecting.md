

Руководство по T-FLEX CAD Open API

# SurfaceSplineDataSelfIntersecting - свойство  
  
---  
  
Признак самопересечения сплайна

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool SelfIntersecting { get; set; }
```
```vb
Public Property SelfIntersecting As Boolean
	Get
	Set
```
```cpp
public:
property bool SelfIntersecting {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Если этот признак не определён, то сплайновая поверхность считается не самопересекающейся

#### Ссылки

[SurfaceSplineData - ](T_TFlex_Model_Model3D_Geometry_SurfaceSplineData.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)