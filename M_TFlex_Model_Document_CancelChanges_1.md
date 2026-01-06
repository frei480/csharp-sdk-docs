

Руководство по T-FLEX CAD Open API

# DocumentCancelChanges(Boolean) - метод  
    
Отменить все изменения и закрыть блок изменения документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void CancelChanges(
	bool regenerate
)
```




#### Параметры

regenerate [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

Функция закрывает блок изменения документа, открытый при помощи функции [BeginChanges(String)](M_TFlex_Model_Document_BeginChanges.md) с отменой всех произведённых изменений.

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[CancelChanges - перегрузка](Overload_TFlex_Model_Document_CancelChanges.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)