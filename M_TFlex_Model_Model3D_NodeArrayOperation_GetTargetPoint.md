

Руководство по T-FLEX CAD Open API

# NodeArrayOperationGetTargetPoint - метод  
    
Получить целевую точку массива по номеру

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D GetTargetPoint(
	int Index
)
```
```vb
Public Function GetTargetPoint ( 
	Index As Integer
) As ModelPoint3D
```
```cpp
public:
ModelPoint3D^ GetTargetPoint(
	int Index
)
```


#### Параметры

Index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер целевой точки

#### Возвращаемое значение

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Целевые точки нумеруются с нуля. Если индекс отрицательный или превышает количество целевых точек, то результат не определён

#### Ссылки

[NodeArrayOperation - ](T_TFlex_Model_Model3D_NodeArrayOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)