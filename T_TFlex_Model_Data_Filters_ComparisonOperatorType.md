

Руководство по T-FLEX CAD Open API

# ComparisonOperatorType - перечисление  
    
Тип оператора сравнения

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public enum ComparisonOperatorType
```
```vb
Public Enumeration ComparisonOperatorType
```
```cpp
public enum class ComparisonOperatorType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Equal | 0 | = |
| NotEqual | 1 | != |
| IsOneOf | 2 | Входит в список |
| IsNotOneOf | 3 | Не входит в список |
| GreaterThan | 4 | > |
| LessThan | 5 | < |
| GreaterThanOrEqual | 6 | >= |
| LessThanOrEqual | 7 | <= |
| IsNull | 8 | Не содержит данных |
| IsNotNull | 9 | Содержит какие-либо данные |
| ContainsSubstring | 10 | Содержит |
| NotContainSubstring | 11 | Не содержит |
| StartsWithSubstring | 12 | Начинается с |
| EndsWithSubstring | 13 | Заканчивается на |
| IsEmptyString | 14 | Не содержит текст |
| IsNotEmptyString | 15 | Содержит текст |
| MatchMask | 16 | Соответствует маске |
| NotMatchMask | 17 | Не соответствует маске |
  
#### Ссылки

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)