

Руководство по T-FLEX CAD Open API

# DiagnosticsStartGroup - метод  
    
Открыть группу сообщений

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void StartGroup()
```




Для того, чтобы избежать множества звуковых сигналов об ошибках, в системе введено понятие "группы сообщений". Звуковой сигнал об ошибке выдаётся один раз внутри группы сообщений. открытую группу сообщений необходимо закрыть при помощи метода [EndGroup](M_TFlex_Model_Diagnostics_EndGroup.md). Группы могут быть вложенными.

#### Ссылки

[Diagnostics - ](T_TFlex_Model_Diagnostics.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)