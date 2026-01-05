

Руководство по T-FLEX CAD Open API

# IncludeInBom - перечисление  
  
---  
  
Типы включения в спецификации

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum IncludeInBom
```
```vb
Public Enumeration IncludeInBom
```
```cpp
public enum class IncludeInBom
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| NotIncluded | 0 | Не включать |
| WithoutEmbeddedElements | 1 | Без вложенных элементов |
| WithEmbeddedElements | 2 | С вложенными элементами |
| OnlyEmbeddedElements | 3 | Только вложенные элементы |
| WithBom | 4 | Со спецификацией |
| OnlyBom | 5 | Только спецификацию |
| WithParametricBom | 6 | С параметрической спецификацией |
| OnlyParametricBom | 7 | Только параметрическая спецификация |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)