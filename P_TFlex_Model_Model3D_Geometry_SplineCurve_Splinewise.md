

Руководство по T-FLEX CAD Open API

# SplineCurveSplinewise - свойство  
    
Описание интерполяционного сплайна по набору точек, через которые проходит сплайн, по параметрам кривой в этих точках и условиям на концах

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public virtual SplinewiseData Splinewise { get; set; }
```
```vb
Public Overridable Property Splinewise As SplinewiseData
	Get
	Set
```
```cpp
public:
virtual property SplinewiseData^ Splinewise {
	SplinewiseData^ get ();
	void set (SplinewiseData^ value);
}
```


#### Значение свойства

[SplinewiseData](T_TFlex_Model_Model3D_Geometry_SplinewiseData.md)

#### Реализации

[BaseSplineCurveSplinewise](P_TFlex_Model_Model3D_Geometry_BaseSplineCurve_Splinewise.md)

Не все сплайны могут вернуть это представление

#### Ссылки

[SplineCurve - ](T_TFlex_Model_Model3D_Geometry_SplineCurve.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)