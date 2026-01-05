

Руководство по T-FLEX CAD Open API

# ModelSplineSurfaceSplinewise - свойство  
  
---  
  
Получить описание интерполяционной сплайновой поверхности по набору точек, через которые проходит сплайновая поверхность, по параметрам поверхности в этих точках и условиям на концах

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public virtual SurfaceSplinewiseData Splinewise { get; }
```
```vb
Public Overridable ReadOnly Property Splinewise As SurfaceSplinewiseData
	Get
```
```cpp
public:
virtual property SurfaceSplinewiseData^ Splinewise {
	SurfaceSplinewiseData^ get ();
}
```


#### Значение свойства

[SurfaceSplinewiseData](T_TFlex_Model_Model3D_Geometry_SurfaceSplinewiseData.md)

#### Реализации

[BaseSplineSurfaceSplinewise](P_TFlex_Model_Model3D_Geometry_BaseSplineSurface_Splinewise.md)

Не все сплайновые поверхности могут вернуть это представление

#### Ссылки

[ModelSplineSurface - ](T_TFlex_Model_Model3D_Geometry_ModelSplineSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)