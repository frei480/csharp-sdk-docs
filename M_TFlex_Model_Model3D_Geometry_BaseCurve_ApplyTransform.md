

Руководство по T-FLEX CAD Open API

# BaseCurveApplyTransform - метод  
    
Трансформация кривой

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Curve ApplyTransform(
	TransformationMatrix transformation
)
```
```vb
Public Function ApplyTransform ( 
	transformation As TransformationMatrix
) As Curve
```
```cpp
public:
Curve^ ApplyTransform(
	TransformationMatrix^ transformation
)
```


#### Параметры

transformation [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)
    Матрица преобразования

#### Возвращаемое значение

[Curve](T_TFlex_Model_Model3D_Geometry_Curve.md)

Создаётся новая кривая

#### Ссылки

[BaseCurve - ](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)