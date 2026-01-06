

Руководство по T-FLEX CAD Open API

# ModelSplineCurveSplinewise - свойство  
    
Получить описание интерполяционного сплайна по набору точек, через которые проходит сплайн, по параметрам кривой в этих точках и условиям на концах

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public virtual SplinewiseData Splinewise { get; }
```
```vb
Public Overridable ReadOnly Property Splinewise As SplinewiseData
	Get
```
```cpp
public:
virtual property SplinewiseData^ Splinewise {
	SplinewiseData^ get ();
}
```


#### Значение свойства

[SplinewiseData](T_TFlex_Model_Model3D_Geometry_SplinewiseData.md)

#### Реализации

[BaseSplineCurveSplinewise](P_TFlex_Model_Model3D_Geometry_BaseSplineCurve_Splinewise.md)

Не все сплайны могут вернуть это представление

#### Ссылки

[ModelSplineCurve - ](T_TFlex_Model_Model3D_Geometry_ModelSplineCurve.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)