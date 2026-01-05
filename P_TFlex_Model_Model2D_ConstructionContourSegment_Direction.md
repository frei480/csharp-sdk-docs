

Руководство по T-FLEX CAD Open API

# ConstructionContourSegmentDirection - свойство  
  
---  
  
Направление сегмента контура

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool Direction { get; set; }
```
```vb
Public Property Direction As Boolean
	Get
	Set
```
```cpp
public:
property bool Direction {
	bool get ();
	void set (bool value);
}
```


#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)true если сегмент контура направлен по положительному направлению линии построения, false в противном случае

Параметр имеет смысл только в случае если заданы одновременно два узла и линия построения. Если любой из элементов не задан, то параметр имеет значение true.

#### Ссылки

[ConstructionContourSegment - ](T_TFlex_Model_Model2D_ConstructionContourSegment.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)