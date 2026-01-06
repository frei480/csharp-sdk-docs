

Руководство по T-FLEX CAD Open API

# ConstraintPointType - перечисление  
    
Типы характерных точек кривых

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum ConstraintPointType
```
```vb
Public Enumeration ConstraintPointType
```
```cpp
public enum class ConstraintPointType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Start | 0 | Начало |
| End | 1 | Конец |
| Center | 2 | Центр эллиптических кривых |
| Middle | 3 | Середина |
| EllipseMajor | 4 | Точка первой полуоси эллипса |
| Undefined | -1 | Неизвестная точка. Требуется в ограничениях, которые используются на кривой в целом. |
| SplinePoint | 10,000 | Номер узла(контрольной точки) сплайна. |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)