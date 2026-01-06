

Руководство по T-FLEX CAD Open API

# TopolArrayInsert - метод  
    
Вставить элемент перед номером

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int Index,
	ModelTopol geom
)
```
```vb
Public Sub Insert ( 
	Index As Integer,
	geom As ModelTopol
)
```
```cpp
public:
void Insert(
	int Index, 
	ModelTopol^ geom
)
```


#### Параметры

Index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер элемента
geom [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)
    Вставляемый элемент

Элементы нумеруются от нуля. Если индекс отрицательный или превышает количество элементов, то результат не определён

#### Ссылки

[TopolArray - ](T_TFlex_Model_Model3D_TopolArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)