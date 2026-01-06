

Руководство по T-FLEX CAD Open API

# ParameterizationType - перечисление  
    
Тип последовательности узлов

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum ParameterizationType
```
```vb
Public Enumeration ParameterizationType
```
```cpp
public enum class ParameterizationType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Unset | 0 | Тип последовательности не определён |
| NonUniform | 1 | Неравномерная параметризация |
| Uniform | 2 | Равномерная параметризация |
| QuasiUniform | 3 | Первый и последний узлы кратности = Степень сплайна + 1, остальные узлы имеют кратность = 1, с разбиением на равные промежутки |
| PiecewiseBezier | 4 | Первый и последний узлы кратности = Степень сплайна + 1, остальные узлы имеют кратность = Степень сплайна, с разбиением на равные промежутки |
| BezierEnds | 5 | Первый и последний узлы кратности = Степень сплайна + 1. Остальные узлы расположены неравномерно |
| SmoothSeam | 6 | Параметризация для замкнутых периодических сплайнов |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)