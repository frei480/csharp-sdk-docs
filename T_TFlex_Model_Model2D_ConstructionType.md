

Руководство по T-FLEX CAD Open API

# ConstructionType - перечисление  
  
---  
  
Подтипы линий построения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum ConstructionType
```
```vb
Public Enumeration ConstructionType
```
```cpp
public enum class ConstructionType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Undefined | 0 | Не определён |
| LineConstruction | 1 | Линия построения - прямая. Класс [LineConstruction](T_TFlex_Model_Model2D_LineConstruction.md) |
| CircleConstruction | 2 | Линия построения - окружность. Класс [CircleConstruction](T_TFlex_Model_Model2D_CircleConstruction.md) |
| EllipseConstruction | 3 | Линия построения - эллипс. Класс [EllipseConstruction](T_TFlex_Model_Model2D_EllipseConstruction.md) |
| PathConstruction | 4 | Линия построения - путь. Класс [PathConstruction](T_TFlex_Model_Model2D_PathConstruction.md) |
| CopyConstruction | 5 | Линия построения, полученная ассоциативным копированием. Класс [CopyConstruction](T_TFlex_Model_Model2D_CopyConstruction.md) |
| OffsetConstruction | 6 | Эквидистанта. Класс [OffsetConstruction](T_TFlex_Model_Model2D_OffsetConstruction.md) |
| SplineConstruction | 7 | Сплайн. Класс [SplineConstruction](T_TFlex_Model_Model2D_SplineConstruction.md) |
| FunctionConstruction | 8 | Функция. Класс [FunctionConstruction](T_TFlex_Model_Model2D_FunctionConstruction.md) |
| SymmetryConstruction | 9 | Линия построения, симметричная относительно оси. Класс [!:TFlex::Model::Model2D::SymmetryConstruction] |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)