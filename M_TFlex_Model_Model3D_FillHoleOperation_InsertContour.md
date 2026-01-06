

Руководство по T-FLEX CAD Open API

# FillHoleOperationInsertContour - метод  
    
Вставить контур

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FillHoleOperationContour InsertContour(
	int contourIndex,
	ModelWire wire
)
```
```vb
Public Function InsertContour ( 
	contourIndex As Integer,
	wire As ModelWire
) As FillHoleOperationContour
```
```cpp
public:
FillHoleOperationContour^ InsertContour(
	int contourIndex, 
	ModelWire^ wire
)
```


#### Параметры

contourIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс добавляемого контура (начинается с 0)
wire [ModelWire](T_TFlex_Model_Model3D_Geometry_ModelWire.md)
    

#### Возвращаемое значение

[FillHoleOperationContour](T_TFlex_Model_Model3D_FillHoleOperation_Contour.md)

#### Ссылки

[FillHoleOperation - ](T_TFlex_Model_Model3D_FillHoleOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)