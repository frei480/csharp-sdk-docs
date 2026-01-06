

Руководство по T-FLEX CAD Open API

# DocumentEndChanges - метод  
    
Применить изменения и закрыть блок изменения документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ChangesResult EndChanges()
```
```vb
Public Function EndChanges As ChangesResult
```
```cpp
public:
ChangesResult EndChanges()
```


#### Возвращаемое значение

[ChangesResult](T_TFlex_Model_ChangesResult.md)Результат применения изменений

Функция закрывает блок изменения документа, открытый при помощи функции [BeginChanges(String)](M_TFlex_Model_Document_BeginChanges.md) Функция автоматически применяет все изменения блока если они являются корректными. В таком случае возвращаемое значение равно OK. Иначе все изменения отменяются.

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[EndChanges - перегрузка](Overload_TFlex_Model_Document_EndChanges.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)