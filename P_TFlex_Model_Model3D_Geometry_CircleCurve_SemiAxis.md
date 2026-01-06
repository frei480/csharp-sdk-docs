

Руководство по T-FLEX CAD Open API

# CircleCurveSemiAxis - свойство  
    
Полуось, от которой откладывается угол окружности

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public virtual BaseDirection SemiAxis { get; set; }
```
```vb
Public Overridable Property SemiAxis As BaseDirection
	Get
	Set
```
```cpp
public:
virtual property BaseDirection^ SemiAxis {
	BaseDirection^ get ();
	void set (BaseDirection^ value);
}
```


#### Значение свойства

[BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)

#### Реализации

[BaseCircleCurveSemiAxis](P_TFlex_Model_Model3D_Geometry_BaseCircleCurve_SemiAxis.md)

Очевидно, что эта полуось лежит в плоскости окружности

#### Ссылки

[CircleCurve - ](T_TFlex_Model_Model3D_Geometry_CircleCurve.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)