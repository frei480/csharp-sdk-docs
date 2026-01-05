

Руководство по T-FLEX CAD Open API

# Path2DPathSegmentsSetInsert - метод  
  
---  
  
Вставить сегмент перед номером

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int Index,
	Path2DPathSegmentsSetSegment segment
)
```
```vb
Public Sub Insert ( 
	Index As Integer,
	segment As Path2DPathSegmentsSetSegment
)
```
```cpp
public:
void Insert(
	int Index, 
	Path2DPathSegmentsSetSegment^ segment
)
```


#### Параметры

Index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер сегмента
segment [Path2DPathSegmentsSetSegment](T_TFlex_Model_Model3D_Path2DPath_SegmentsSet_Segment.md)
    Вставляемый сегмент

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат не определён

#### Ссылки

[Path2DPathSegmentsSet - ](T_TFlex_Model_Model3D_Path2DPath_SegmentsSet.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)