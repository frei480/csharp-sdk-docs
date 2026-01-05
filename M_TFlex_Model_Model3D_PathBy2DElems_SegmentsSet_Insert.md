

Руководство по T-FLEX CAD Open API

# PathBy2DElemsSegmentsSetInsert - метод  
  
---  
  
Вставить сегмент перед номером

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int Index,
	PathBy2DElemsSegmentsSetSegment segment
)
```
```vb
Public Sub Insert ( 
	Index As Integer,
	segment As PathBy2DElemsSegmentsSetSegment
)
```
```cpp
public:
void Insert(
	int Index, 
	PathBy2DElemsSegmentsSetSegment^ segment
)
```


#### Параметры

Index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер сегмента
segment [PathBy2DElemsSegmentsSetSegment](T_TFlex_Model_Model3D_PathBy2DElems_SegmentsSet_Segment.md)
    Вставляемый сегмент

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат не определён

#### Ссылки

[PathBy2DElemsSegmentsSet - ](T_TFlex_Model_Model3D_PathBy2DElems_SegmentsSet.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)