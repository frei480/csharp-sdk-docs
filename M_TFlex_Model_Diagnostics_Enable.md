

Руководство по T-FLEX CAD Open API

# DiagnosticsEnable - метод  
    
Разрешить или запретить добавление сообщений в контейнер.

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool Enable(
	bool enable
)
```
```vb
Public Function Enable ( 
	enable As Boolean
) As Boolean
```
```cpp
public:
bool Enable(
	bool enable
)
```


#### Параметры

enable [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    true, если необходимо разрешить выдачу сообщений; false в случае запрета

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Значение параметра, которое было установлено до вызова данного метода

В некоторых случаях полезно запретить вывод сообщений в окно диагностики системы. С этой целью можно воспользоваться данным методом. После завершения действий, связанных с данным запретом, необходимо установить данный параметр в значение, которое он имел до этого.

#### Ссылки

[Diagnostics - ](T_TFlex_Model_Diagnostics.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)