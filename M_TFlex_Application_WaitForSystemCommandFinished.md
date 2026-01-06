

Руководство по T-FLEX CAD Open API

# ApplicationWaitForSystemCommandFinished - метод  
    
Ожидание завершения команды

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static void WaitForSystemCommandFinished(
	string commandName,
	SystemCommandFinishedCallback commandFinishedCallback
)
```
```vb
Public Shared Sub WaitForSystemCommandFinished ( 
	commandName As String,
	commandFinishedCallback As SystemCommandFinishedCallback
)
```
```cpp
public:
static void WaitForSystemCommandFinished(
	String^ commandName, 
	SystemCommandFinishedCallback^ commandFinishedCallback
)
```


#### Параметры

commandName [String](https://learn.microsoft.com/dotnet/api/system.string)
    
commandFinishedCallback [SystemCommandFinishedCallback](T_TFlex_SystemCommandFinishedCallback.md)
    

#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)