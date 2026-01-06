

Руководство по T-FLEX CAD Open API

# TransformationMatrixMultiply(BasePoint3D, TransformationMatrix) - оператор  
  **Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Point3D operator *(
	BasePoint3D point,
	TransformationMatrix tr
)
```
```vb
Public Shared Operator * ( 
	point As BasePoint3D,
	tr As TransformationMatrix
) As Point3D
```
```cpp
public:
static Point3D^ operator *(
	BasePoint3D^ point, 
	TransformationMatrix^ tr
)
```


#### Параметры

point [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    
tr [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)
    

#### Возвращаемое значение

[Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)

#### Ссылки

[TransformationMatrix - ](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)

[Multiply - перегрузка](Overload_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)