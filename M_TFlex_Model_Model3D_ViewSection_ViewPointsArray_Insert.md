

Руководство по T-FLEX CAD Open API

# ViewSectionViewPointsArrayInsert - метод  
    
Вставить точку перед номером

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int Index,
	ModelPoint3D geom
)
```
```vb
Public Sub Insert ( 
	Index As Integer,
	geom As ModelPoint3D
)
```
```cpp
public:
void Insert(
	int Index, 
	ModelPoint3D^ geom
)
```


#### Параметры

Index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки
geom [ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)
    

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат неопределён

#### Ссылки

[ViewSectionViewPointsArray - ](T_TFlex_Model_Model3D_ViewSection_ViewPointsArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)