

Руководство по T-FLEX CAD Open API

# LineTypes - перечисление  
  
---  
  
Типы привязок прямых

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum LineTypes
```
```vb
Public Enumeration LineTypes
```
```cpp
public enum class LineTypes
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Undefined | 0 | Не определена |
| Horizontal | 1 | Горизонталь |
| Vertical | 2 | Вертикаль |
| Parallel | 3 | Параллельная прямой |
| OnAngleToLineThroughNode | 4 | Проходящая через узел, под углом к другой прямой |
| TangentToCircle | 5 | Через узел, касательная к окружности |
| ThroughNodes | 6 | Через два узла |
| TangentToCircles | 7 | Касательная к двум окружностям |
| Symmetric | 8 | Симметричная другой прямой относительно оси |
| AxisOfLines | 9 | Ось симметрии двух прямых |
| TangentToCircleOnAngle | 10 | Касательная к окружности, под углом к другой прямой |
| ParallelThroughNode | 11 | Параллельная другой прямой, проходящая через узел |
| ParallelTangentToCircle | 12 | Параллельная другой прямой, касательная к окружности |
| VerticalThroughNode | 13 | Вертикальная прямая, проходящая через узел |
| HorizontalThroughNode | 14 | Горизонтальная прямая, проходящая через узел |
| PerpendicularThroughNode | 15 | Перпендикулярная другой прямой, проходящая через узел |
| OnAngleThroughNode | 16 | Проходящая через узел, под углом к горизонтали |
| DividingNodes | 17 | Перпендикулярная отрезку между двумя узлами, делящая отрезок в заданной пропорции |
| ThoughNodeTangentToEllipse | 18 | Проходящая через узел, касательная к эллипсу |
| ParallelTangentToEllipse | 19 | Параллельная другой прямой, касательная к эллипсу |
| ParallelTangentToPolyline | 20 | Параллельная другой прямой, касательная к полилинии |
| ThoughNodeTangentToPolyline | 21 | Проходящая через узел, касательная к полилинии |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)