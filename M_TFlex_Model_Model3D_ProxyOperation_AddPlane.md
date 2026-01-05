

Руководство по T-FLEX CAD Open API

# ProxyOperationAddPlane - метод  
  
---  
  
Добавить плоскость в геометрию

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
protected bool AddPlane(
	int index,
	BasePlane plane
)
```
```vb
Protected Function AddPlane ( 
	index As Integer,
	plane As BasePlane
) As Boolean
```
```cpp
protected:
bool AddPlane(
	int index, 
	BasePlane^ plane
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Допустимое значение 0,1,2
plane [BasePlane](T_TFlex_Model_Model3D_Geometry_BasePlane.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Вызывается только в функции MakeGeometry

#### Ссылки

[ProxyOperation - ](T_TFlex_Model_Model3D_ProxyOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)