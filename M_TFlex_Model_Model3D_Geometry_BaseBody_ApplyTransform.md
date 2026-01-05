

Руководство по T-FLEX CAD Open API

# BaseBodyApplyTransform - метод  
  
---  
  
Трансформация геометрии тела

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Body ApplyTransform(
	TransformationMatrix transformation
)
```
```vb
Public Function ApplyTransform ( 
	transformation As TransformationMatrix
) As Body
```
```cpp
public:
Body^ ApplyTransform(
	TransformationMatrix^ transformation
)
```


#### Параметры

transformation [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)
    Матрица преобразования

#### Возвращаемое значение

[Body](T_TFlex_Model_Model3D_Geometry_Body.md)

Создаётся новое тело

#### Ссылки

[BaseBody - ](T_TFlex_Model_Model3D_Geometry_BaseBody.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)