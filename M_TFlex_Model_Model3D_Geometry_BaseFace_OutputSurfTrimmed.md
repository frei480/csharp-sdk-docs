

Руководство по T-FLEX CAD Open API

# BaseFaceOutputSurfTrimmed - метод  
    
Возвращает обрезанную поверхность

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
SurfTrimmedData OutputSurfTrimmed(
	double tolerance
)
```
```vb
Function OutputSurfTrimmed ( 
	tolerance As Double
) As SurfTrimmedData
```
```cpp
SurfTrimmedData^ OutputSurfTrimmed(
	double tolerance
)
```


#### Параметры

tolerance [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Максимально допустимое расстояние между поверхностью грани и аппроксимирующей сплайновой поверхностью

#### Возвращаемое значение

[SurfTrimmedData](T_TFlex_Model_Model3D_Geometry_SurfTrimmedData.md)

Рекомендуемая точность = 0.00001

#### Ссылки

[BaseFace - ](T_TFlex_Model_Model3D_Geometry_BaseFace.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)