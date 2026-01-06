

Руководство по T-FLEX CAD Open API

# InputControlFocusLostBehavior - перечисление  
    
Поведение при потере фокуса

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public enum InputControlFocusLostBehavior
```




| Имя члена | Значение | Описание |
| --- | --- | --- |
| None | 0 | При потере фокуса действие не требуется |
| ApplyOnly | 1 | При потере фокуса попробовать применить изменения |
| EndUserEdit | 2 | При потере фокуса попробовать применить изменения. В случае неудачи, откатить до предыдущео состояния. |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)