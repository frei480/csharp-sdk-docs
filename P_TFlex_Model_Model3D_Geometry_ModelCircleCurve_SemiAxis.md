

Руководство по T-FLEX CAD Open API

# ModelCircleCurveSemiAxis - свойство  
  
---  
  
Получить полуось, от которой откладывается угол окружности

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public virtual BaseDirection SemiAxis { get; }
```
```vb
Public Overridable ReadOnly Property SemiAxis As BaseDirection
	Get
```
```cpp
public:
virtual property BaseDirection^ SemiAxis {
	BaseDirection^ get ();
}
```


#### Значение свойства

[BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)

#### Реализации

[BaseCircleCurveSemiAxis](P_TFlex_Model_Model3D_Geometry_BaseCircleCurve_SemiAxis.md)

Очевидно, что эта полуось лежит в плоскости окружности

#### Ссылки

[ModelCircleCurve - ](T_TFlex_Model_Model3D_Geometry_ModelCircleCurve.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)