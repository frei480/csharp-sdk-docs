

Руководство по T-FLEX CAD Open API

# ProxyOperationAddPoint - метод  
    
Добавить точку в геометрию

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
protected bool AddPoint(
	int index,
	BasePoint3D point
)
```
```vb
Protected Function AddPoint ( 
	index As Integer,
	point As BasePoint3D
) As Boolean
```
```cpp
protected:
bool AddPoint(
	int index, 
	BasePoint3D^ point
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Допустимое значение 0,1,2
point [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Вызывается только в функции MakeGeometry

#### Ссылки

[ProxyOperation - ](T_TFlex_Model_Model3D_ProxyOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)