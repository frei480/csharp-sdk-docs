

Руководство по T-FLEX CAD Open API

# PluginDeletingObjectParentsEventHandler - метод  
  
---  
  
Обработчик события, возникающего перед удалением объекта модели для получания дополнтиельных зависимых объектов для удаления

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual void DeletingObjectParentsEventHandler(
	DeletingObjectParentsEventArgs args
)
```
```vb
Protected Overridable Sub DeletingObjectParentsEventHandler ( 
	args As DeletingObjectParentsEventArgs
)
```
```cpp
protected:
virtual void DeletingObjectParentsEventHandler(
	DeletingObjectParentsEventArgs^ args
)
```


#### Параметры

args [DeletingObjectParentsEventArgs](T_TFlex_DeletingObjectParentsEventArgs.md)
    Аргументы события

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)