

Руководство по T-FLEX CAD Open API

# NumericInputControlState - перечисление  
    
Определяет состояние NumericInputControl

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public enum NumericInputControlState
```
```vb
Public Enumeration NumericInputControlState
```
```cpp
public enum class NumericInputControlState
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| NoVariable | 0 | Введено числовое значение |
| ValidVariable | 1 | Введена существующая переменная |
| NewVariableUnknownValue | 2 | Введена новая переменная без значения |
| NewVariableKnownValue | 3 | Введена новая переменная с известным значением. Используется для выражений. |
| Error | 4 | Во время определения значения произошла ошибка |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)