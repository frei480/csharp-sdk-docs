

Руководство по T-FLEX CAD Open API

# FaceOutputSurfTrimmed - метод  
    
Возвращает обрезанную поверхность

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SurfTrimmedData OutputSurfTrimmed(
	double tolerance
)
```
```vb
Public Function OutputSurfTrimmed ( 
	tolerance As Double
) As SurfTrimmedData
```
```cpp
public:
virtual SurfTrimmedData^ OutputSurfTrimmed(
	double tolerance
) sealed
```


#### Параметры

tolerance [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Максимально допустимое расстояние между поверхностью грани и аппроксимирующей сплайновой поверхностью

#### Возвращаемое значение

[SurfTrimmedData](T_TFlex_Model_Model3D_Geometry_SurfTrimmedData.md)

#### Реализации

[BaseFaceOutputSurfTrimmed(Double)](M_TFlex_Model_Model3D_Geometry_BaseFace_OutputSurfTrimmed.md)

Рекомендуемая точность = 0.00001

#### Ссылки

[Face - ](T_TFlex_Model_Model3D_Geometry_Face.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)