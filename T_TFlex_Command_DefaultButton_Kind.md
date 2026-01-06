

Руководство по T-FLEX CAD Open API

# DefaultButtonKind - перечисление  
    
Перечислитель стандартных кнопок

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum Kind
```
```vb
Public Enumeration Kind
```
```cpp
public enum class Kind
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| OK | 0 | Кнопка принятия команды |
| Cancel | 1 | Кнопка отмены команды |
| Exit | 2 | Кнопка выхода из команды |
| Parameters | 3 | Кнопка вызова диалога параметров |
| Edit | 4 | Кнопка вызова команды "Изменить" |
| Variables | 5 | Кнопка вызова диалога переменных |
| SelectNearbyElement | 6 | Кнопка выбора другого ближайщего элемента |
| DestroyBinding | 7 | Кнопка разрушения привязки |
| SelectFragment | 8 | Кнопка выбора 2D или 3D фрагмента |
| RepeatPrevious | 9 | Кнопка потвора предыдущего фрагмента |
| SetName | 10 | Кнопка установки имени |
| SelectAllElements | 11 | Кнопка выбора всех элементов |
| Axis | 12 | Кнопка перемещения вдоль произвольной оси |
| RepeatEndlessly | 13 | Кнопка бесконечного повтора вставки 3D-фрагмента |
| Open | 14 | Кнопка открытия внешнего файла |
| CreateLineText | 15 | Кнопка создания однострочного текста |
| DeselectCS | 16 | Кнопка отмены выборе системы координат |
| BooleanAddition | 17 | Кнопка сложения тел |
| BooleanSubtraction_A_B | 18 | Кнопка вычитания(a - b) тел |
| BooleanIntersection | 19 | Кнопка пересечение тел |
| SelectFirstBody | 20 | Кнопка выбора первого тела |
| SelectSecondBody | 21 | Кнопка выбора второго тела |
| SelectFirstDirection | 22 | Кнопка первой точки направления |
| SelectEndFirstDirection | 23 | Кнопка выбора конечной точки направления |
| SelectPointForLcs | 24 | Кнопка выбора точки для создания исходной системы координат |
| SelectSourceLcs | 25 | Кнопка выбора исходной системы координат |
| SelectTargetLcs | 26 | Кнопка выбора целевой системы координат |
| CreateResult | 27 | Кнопка создания результата |
| TurnLcsAroundAxisX | 28 | Кнопка поворота системы координат вокруг оси X на 90° |
| TurnLcsAroundAxisY | 29 | Кнопка поворота системы координат вокруг оси Y на 90° |
| TurnLcsAroundAxisZ | 30 | Кнопка поворота системы координат вокруг оси Z на 90° |
| SelectAllSceneBodies | 31 | Кнопка выбора всех тел в текущей сцене |
| SelectElementsForProjection | 32 | Кнопка выбора элементов модели для проецирования |
| TurnAxisCyclically | 33 | Кнопка циклического поворота системы координат |
| CreateByWorkplane | 34 | Кнопка создания по рабочей плоскости (планировка) |
| CreateParagraphText | 35 | Кнопка создания параграф-текста |
| CreateStandardViews | 36 | Кнопка создания набора стандартных видов |
| CreateMultiLineText | 37 | Кнопка создания многострочного текста |
| CreateTable | 38 | Кнопка создания таблицы |
| PreviewResult | 39 | Кнопка предварительного просмотра результата операции |
| SelectPointForTargetLcs | 40 | Кнопка выбора точки для создания целевой системы координат |
| CreateFragmentInContext | 41 | Кнопка создания нового фрагмента в контексте сборки |
| CreateFragment | 42 | Кнопка создания фрагмента |
| SelectSecondFaces | 43 | Кнопка выбора граней второго набора |
| SelectFirstFaces | 44 | Кнопка выбора граней первого набора |
| SetRotationAroundAxis | 45 | Кнопка установки вращения вокруг произвольной оси |
| SelectPoint | 46 | Кнопка выбора точки |
| SelectSplitBodies | 47 | Кнопка выбора рассекаемых тел |
| CopyPropertiesFromElement | 48 | Кнопка копирования параметров с существующего элемента |
| BooleanSubtraction_B_A | 49 | Кнопка вычитания(b - a) тел |
| Group | 50 | Кнопка вызова команды "Сгруппировать" |
| Ungroup | 51 | Кнопка вызова команды "Разгруппировать" |
| SelectElementsForStyleset | 52 | Кнопка выбора элементов модели для задания стиля отображения |
| CreateAssociativeFragmentCopy | 53 | Кнопка создания ассоциативной копии фрагмента |
| Delete | 54 | Кнопка вызова команды "Удалить" |
  
#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)