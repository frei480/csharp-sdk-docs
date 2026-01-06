

Руководство по T-FLEX CAD Open API

# ProxyObjectPropertyChange - перечисление  
    
Перечислитель действий при изменении свойств прокси объекта

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected enum PropertyChange
```
```vb
Protected Enumeration PropertyChange
```
```cpp
protected enum class PropertyChange
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Nothing | 0 | Ничего не делать |
| WeakChange | 1 | Незначительные изменения |
| UpdateScene | 2 | Обновить сцену |
| ReloadInScene | 4 | Загрузить в сцену |
| Regenerate | 8 | Пересчитать модель |
| ChangeTree | 16 | Изменить дерево |
| ChangeMaterial | 32 | Изменить материал |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)