

Руководство по T-FLEX CAD Open API

# RelativeType - перечисление  
    
Типы задания узла, заданного относительно другого узла

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum RelativeType
```
```vb
Public Enumeration RelativeType
```
```cpp
public enum class RelativeType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Undefined | 0 | Не определён |
| Offset | 1 | Смещение, относительно заданного узла |
| OnConstruction | 2 | На линии построения, по расстоянию до заданного узла |
| ByParameter | 3 | Заданние параметром на линии построения |
| EndOfPolyline | 4 | На конце полилинии |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)