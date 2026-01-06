

Руководство по T-FLEX CAD Open API

# TransformationMatrixMultiply(BaseBody, TransformationMatrix) - оператор  
  **Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Body operator *(
	BaseBody body,
	TransformationMatrix tr
)
```
```vb
Public Shared Operator * ( 
	body As BaseBody,
	tr As TransformationMatrix
) As Body
```
```cpp
public:
static Body^ operator *(
	BaseBody^ body, 
	TransformationMatrix^ tr
)
```


#### Параметры

body [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)
    
tr [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)
    

#### Возвращаемое значение

[Body](T_TFlex_Model_Model3D_Geometry_Body.md)

#### Ссылки

[TransformationMatrix - ](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)

[Multiply - перегрузка](Overload_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)