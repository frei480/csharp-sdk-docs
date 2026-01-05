

Руководство по T-FLEX CAD Open API

# TransformationMatrixMultiply(BaseDirection, TransformationMatrix) - оператор  
  
---  
**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Direction operator *(
	BaseDirection direction,
	TransformationMatrix tr
)
```
```vb
Public Shared Operator * ( 
	direction As BaseDirection,
	tr As TransformationMatrix
) As Direction
```
```cpp
public:
static Direction^ operator *(
	BaseDirection^ direction, 
	TransformationMatrix^ tr
)
```


#### Параметры

direction [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    
tr [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)
    

#### Возвращаемое значение

[Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)

#### Ссылки

[TransformationMatrix - ](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)

[Multiply - перегрузка](Overload_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)