

Руководство по T-FLEX CAD Open API

# GeometricArrayInsert - метод  
    
Вставить элемент перед номером

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int index,
	Geometry geom
)
```
```vb
Public Sub Insert ( 
	index As Integer,
	geom As Geometry
)
```
```cpp
public:
void Insert(
	int index, 
	Geometry^ geom
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер элемента
geom [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)
    Элемент

Элементы нумеруются от нуля. Если индекс отрицательный или превышает количество элементов, то результат не определён

#### Ссылки

[GeometricArray - ](T_TFlex_Model_Model3D_Geometry_GeometricArray.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)