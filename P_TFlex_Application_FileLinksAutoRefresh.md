

Руководство по T-FLEX CAD Open API

# ApplicationFileLinksAutoRefresh - свойство  
    
Режим обновления файловых ссылок

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static ApplicationFileLinksRefreshMode FileLinksAutoRefresh { get; set; }
```
```vb
Public Shared Property FileLinksAutoRefresh As ApplicationFileLinksRefreshMode
	Get
	Set
```
```cpp
public:
static property ApplicationFileLinksRefreshMode FileLinksAutoRefresh {
	ApplicationFileLinksRefreshMode get ();
	void set (ApplicationFileLinksRefreshMode value);
}
```


#### Значение свойства

[ApplicationFileLinksRefreshMode](T_TFlex_Application_FileLinksRefreshMode.md)

Работает только в режиме пользовательского приложения. См. метод [InitSession(ApplicationSessionSetup)](M_TFlex_Application_InitSession.md)

#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)