

Руководство по T-FLEX CAD Open API

# PluginOnExiting - метод  
  
---  
  
Событие перед закрытием главного окна. Закрытие окна может быть отменено.

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual void OnExiting(
	CancelEventArgs args
)
```
```vb
Protected Overridable Sub OnExiting ( 
	args As CancelEventArgs
)
```
```cpp
protected:
virtual void OnExiting(
	CancelEventArgs^ args
)
```


#### Параметры

args [CancelEventArgs](https://learn.microsoft.com/dotnet/api/system.componentmodel.canceleventargs)
    Аргументы события

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)