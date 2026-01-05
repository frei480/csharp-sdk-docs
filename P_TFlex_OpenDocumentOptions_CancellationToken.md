

Руководство по T-FLEX CAD Open API

# OpenDocumentOptionsCancellationToken - свойство  
  
---  
  
Объект для уведомления о необходимости отмены команды

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public CancellationToken CancellationToken { get; set; }
```
```vb
Public Property CancellationToken As CancellationToken
	Get
	Set
```
```cpp
public:
property CancellationToken CancellationToken {
	CancellationToken get ();
	void set (CancellationToken value);
}
```


#### Значение свойства

[CancellationToken](https://learn.microsoft.com/dotnet/api/system.threading.cancellationtoken)

Может использоваться совместно с для возможности отмены команды как пользователем, так и программно

#### Ссылки

[OpenDocumentOptions - ](T_TFlex_OpenDocumentOptions.md)

[TFlex - пространство имён](N_TFlex.md)