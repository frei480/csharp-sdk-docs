

Руководство по T-FLEX CAD Open API

# DocumentApplyChanges - метод  
  
---  
  
Применить изменения без закрытия блока изменения документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ChangesResult ApplyChanges()
```
```vb
Public Function ApplyChanges As ChangesResult
```
```cpp
public:
ChangesResult ApplyChanges()
```


#### Возвращаемое значение

[ChangesResult](T_TFlex_Model_ChangesResult.md)Результат применения изменений

Функция применяет изменения, сделаные после вызова функции [BeginChanges(String)](M_TFlex_Model_Document_BeginChanges.md)

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[ApplyChanges - перегрузка](Overload_TFlex_Model_Document_ApplyChanges.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)