

Руководство по T-FLEX CAD Open API

# ApplicationInitSession - метод  
    
Инициализация API

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static bool InitSession(
	ApplicationSessionSetup setup
)
```
```vb
Public Shared Function InitSession ( 
	setup As ApplicationSessionSetup
) As Boolean
```
```cpp
public:
static bool InitSession(
	ApplicationSessionSetup^ setup
)
```


#### Параметры

setup [ApplicationSessionSetup](T_TFlex_ApplicationSessionSetup.md)
    Параметры инициализации сессии

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)true в случае успешного завершения

Данный метод необходимо вызвать при инициализации API в случае использования его в отдельном приложении (EXE). При необходимости завершения работы с API до закрытия приложения нужно вызывать метод [ExitSession](M_TFlex_Application_ExitSession.md)

#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)