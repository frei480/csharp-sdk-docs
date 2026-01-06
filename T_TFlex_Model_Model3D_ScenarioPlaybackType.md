

Руководство по T-FLEX CAD Open API

# ScenarioPlaybackType - перечисление  
    
Тип воспроизведения анимации

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum ScenarioPlaybackType
```
```vb
Public Enumeration ScenarioPlaybackType
```
```cpp
public enum class ScenarioPlaybackType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Direct | 0 | Анимация от начала до конца, и стоп (разборка) (по умолчанию) |
| Looped | 1 | Анимация от начала до конца, и обратно (от конца до начала) (разборка - сборка) |
| DirectRepeat | 2 | ptDirect с повтором |
| Revers | 3 | Анимация от конца к началу (сборка) |
| ReversRepeat | 4 | ptReversRepeat с повтором |
| Flash | 5 | Отсутствие анимации |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)