

Руководство по T-FLEX CAD Open API

# TransformationMatrixMultiply(BaseCurve, TransformationMatrix) - оператор  
  **Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Curve operator *(
	BaseCurve curve,
	TransformationMatrix tr
)
```
```vb
Public Shared Operator * ( 
	curve As BaseCurve,
	tr As TransformationMatrix
) As Curve
```
```cpp
public:
static Curve^ operator *(
	BaseCurve^ curve, 
	TransformationMatrix^ tr
)
```


#### Параметры

curve [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)
    
tr [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)
    

#### Возвращаемое значение

[Curve](T_TFlex_Model_Model3D_Geometry_Curve.md)

#### Ссылки

[TransformationMatrix - ](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)

[Multiply - перегрузка](Overload_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)