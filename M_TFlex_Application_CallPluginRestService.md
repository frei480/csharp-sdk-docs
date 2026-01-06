

Руководство по T-FLEX CAD Open API

# ApplicationCallPluginRestService - метод  
    
Вызвать RESTful сервис плагина. Формат входных/выходных данных зависит от конкретного плагина.

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Response CallPluginRestService(
	string pluginName,
	Request request
)
```
```vb
Public Shared Function CallPluginRestService ( 
	pluginName As String,
	request As Request
) As Response
```
```cpp
public:
static Response^ CallPluginRestService(
	String^ pluginName, 
	Request^ request
)
```


#### Параметры

pluginName [String](https://learn.microsoft.com/dotnet/api/system.string)
    
request [Request](T_TFlex_Rest_Request.md)
    

#### Возвращаемое значение

[Response](T_TFlex_Rest_Response.md)

#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)