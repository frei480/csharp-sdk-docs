

Руководство по T-FLEX CAD Open API

# CircleTypes - перечисление  
    
Типы привязок окружностей

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum CircleTypes
```




| Имя члена | Значение | Описание |
| --- | --- | --- |
| Undefined | 0 | Не определён |
| CenterAndRadius | 1 | С центром в узле и заданным радиусом |
| TangentToLineAndNode | 2 | Касательная к прямой, проходящая через узел |
| TangentToCircleAndNode | 3 | Касательная к окружности, проходящая через узел |
| TangentToTwoLines | 4 | Касательная к двум прямым |
| TangentToCircleAndLine | 5 | Касательная к окружности и прямой |
| TangentToTwoCircles | 6 | Касательная к двум окружностям |
| TangentToThreeLines | 7 | Касательная к трём прямым |
| ThreeNodes | 8 | Проходящая через три узла |
| Symmetric | 9 | Симметричная другой окружности относительно оси |
| CenterAndNode | 10 | С центром в узле, проходящая через узел |
| CenterAndLine | 11 | С центром в узле, касательная к прямой |
| CenterAndCircle | 12 | С центром в узле, касательная к окружности |
| CenterAndEllipse | 13 | С центром в узле, касательная к эллипсу |
| TwoNodes | 14 | Проходящая через два узла |
| Offset | 15 | Концентричная исходной окружности на заданном расстоянии |
| TwoNodesTangentToLine | 16 | Проходящая через два узла, касательная к прямой |
| NodeTangentToTwoLines | 17 | Проходящая через узел, касательная к двум прямым |
| TwoNodesTangentToCircle | 18 | Проходящая через два узла, касательная к окружности |
| NodeTangentToLineAndCircle | 19 | Проходящая через узел, касательная к прямой и окружности |
| NodeTangentToTwoCircles | 20 | Проходящая через узел, касательная к двум окружностям |
| TangentToTwoLinesAndCircle | 21 | Касательная к двум прямым и окружности |
| TangentToLineAndTwoCircles | 22 | Касательная к прямой и двум окружностям |
| TangentToThreeCircles | 23 | Касательная к трём окружностям |
| TangentToLineAndPolyline | 24 | Касательная к прямой и сплайну или другой полилинии |
| TangentToCircleAndPolyline | 25 | Касательная к окружности и сплайну или другой полилинии |
| TangentToTwoPolylines | 26 | Касательная к двум сплайнам или другим полилиниям |
| TangentToLineAndEllipse | 27 | Касательная к прямой и эллипсу |
| TangentToCircleAndEllipse | 28 | Касательная к окружности и эллипсу |
| TangentToEllipseAndPolyline | 29 | Касательная к эллипсу и сплайну или другой полилинии |
| TangentToTwoEllipses | 30 | Касательная к двум эллипсам |
| Outline | 31 | Проходящая по линии изображения (окружности или дуге окружности) |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)