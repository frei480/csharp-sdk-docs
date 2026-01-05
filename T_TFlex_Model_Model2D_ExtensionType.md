

Руководство по T-FLEX CAD Open API

# ExtensionType - перечисление  
  
---  
  
Тип способа управления смещением

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum ExtensionType
```
```vb
Public Enumeration ExtensionType
```
```cpp
public enum class ExtensionType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| ByStraightLine | 0 | Линейный |
| KeepCurvature | 1 | Непрерывный по кривизне |
| Mirror | 2 | С отражением |
| ByParameter | 3 | По параметру |
| ByArc | 4 | По дуге |
  
Параметры смещения не доступны для замкнутых сплайнов

#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)