

Руководство по T-FLEX CAD Open API

# SplineSurfacePiecewise - метод  
    
Получить описание интерполяционной сплайновой поверхности по набору точек, через которые проходит сплайновая поверхность, по параметрам поверхности в этих точках и условиям на концах

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public virtual SurfacePiecewiseData Piecewise(
	PiecewiseRepresentation representation
)
```
```vb
Public Overridable Function Piecewise ( 
	representation As PiecewiseRepresentation
) As SurfacePiecewiseData
```
```cpp
public:
virtual SurfacePiecewiseData^ Piecewise(
	PiecewiseRepresentation representation
)
```


#### Параметры

representation [PiecewiseRepresentation](T_TFlex_Model_Model3D_Geometry_PiecewiseRepresentation.md)
    

#### Возвращаемое значение

[SurfacePiecewiseData](T_TFlex_Model_Model3D_Geometry_SurfacePiecewiseData.md)

#### Реализации

[BaseSplineSurfacePiecewise(PiecewiseRepresentation)](M_TFlex_Model_Model3D_Geometry_BaseSplineSurface_Piecewise.md)

Не все сплайновые поверхности могут вернуть это представление

#### Ссылки

[SplineSurface - ](T_TFlex_Model_Model3D_Geometry_SplineSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)