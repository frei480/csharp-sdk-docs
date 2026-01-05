

Руководство по T-FLEX CAD Open API

# LinearDimensionType - перечисление  
  
---  
  
Типы линейных размеров

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum LinearDimensionType
```
```vb
Public Enumeration LinearDimensionType
```
```cpp
public enum class LinearDimensionType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Undefined | 0 | Не задан |
| TwoNodes | 1 | Между двумя узлами |
| TwoNodesHorizontal | 2 | Расстояние между двумя узлами по горизонтали |
| TwoNodesVertical | 3 | Расстояние между двумя узлами по вертикали |
| Segment | 4 | Длина отрезка |
| TwoOutlines | 5 | Расстояние между отрезками |
| TwoConstructions | 6 | Расстояние между прямыми |
| ConstructionAndOutline | 7 | Расстояние между прямой и отрезком |
| ConstructionAndNode | 8 | Расстояние от узла до прямой |
| OutlineAndNode | 9 | Расстояние от узла до отрезка |
| TwoNodesAndLine | 10 | Расстояние между узлами, в направлении, перпендикулярном линии |
| ArcLength | 11 | Длина дуги |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)