

Руководство по T-FLEX CAD Open API

# PluginOnCallRestCallback - метод  
  
---  
  
Событие вызова RESTful сервиса плагина. Формат входных/выходных данных зависит от конкретного плагина.

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual Response OnCallRestCallback(
	Request request
)
```
```vb
Protected Overridable Function OnCallRestCallback ( 
	request As Request
) As Response
```
```cpp
protected:
virtual Response^ OnCallRestCallback(
	Request^ request
)
```


#### Параметры

request [Request](T_TFlex_Rest_Request.md)
    

#### Возвращаемое значение

[Response](T_TFlex_Rest_Response.md)

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)

[!:TFlex::Application::CallPluginRestService]