

Руководство по T-FLEX CAD Open API

# LogWrite(LogSeverity, String, Object) - метод  
  
---  
**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static void Write(
	LogSeverity severity,
	string format,
	params Object[] args
)
```
```vb
Public Shared Sub Write ( 
	severity As LogSeverity,
	format As String,
	ParamArray args As Object()
)
```
```cpp
public:
static void Write(
	LogSeverity severity, 
	String^ format, 
	... array<Object^>^ args
)
```


#### Параметры

severity [LogSeverity](T_TFlex_Log_Severity.md)
    
format [String](https://learn.microsoft.com/dotnet/api/system.string)
    
args [Object](https://learn.microsoft.com/dotnet/api/system.object)
    

#### Ссылки

[Log - ](T_TFlex_Log.md)

[Write - перегрузка](Overload_TFlex_Log_Write.md)

[TFlex - пространство имён](N_TFlex.md)