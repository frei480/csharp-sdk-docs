

Руководство по T-FLEX CAD Open API

# ChangesResult - перечисление  
    
Класс результата пересчёта модели при применении или завершении изменений

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum ChangesResult
```
```vb
Public Enumeration ChangesResult
```
```cpp
public enum class ChangesResult
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| OK | 0 | Нет ошибок |
| ObjectError | 1 | Ошибка пересчёта объекта |
| VariableError | 2 | Ошибка пересчёта переменных модели |
| RecursionError | 3 | Рекурсия при установке взаимосвязей между объектами |
| CompleteError | 4 | Некоторый объект некорректен в смысле полноты и непротиворечивости задания данных |
| UndefinedError | -1 | Неопределённая ошибка |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)