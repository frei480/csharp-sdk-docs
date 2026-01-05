

Руководство по T-FLEX CAD Open API

# RowElementCreateChangesScope - метод  
  
---  
  
Создать область изменений. Запись не будет автоматически пересчитываться при изменениях в ячейках. Вместо этого она пересчитается когда будет вызван Dispose.

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public IDisposable CreateChangesScope()
```
```vb
Public Function CreateChangesScope As IDisposable
```
```cpp
public:
IDisposable^ CreateChangesScope()
```


#### Возвращаемое значение

[IDisposable](https://learn.microsoft.com/dotnet/api/system.idisposable)

Для использования в using.

#### Ссылки

[RowElement - ](T_TFlex_Model_RowElement.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)