

Руководство по T-FLEX CAD Open API

# TermGroupRemoveErrorItems - метод  
    
Удаляет из текущей группы элементы, которые находятся в ошибочном состоянии

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public List<TermGroupItem> RemoveErrorItems(
	bool recursive = true
)
```




#### Параметры

recursive [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean) (Optional)
    Значение true, если требуется удалять элементы в дочерних группах; в противном случае - значение false

#### Возвращаемое значение

[List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)Список элементов группы, удаленных в результате операции

#### Ссылки

[TermGroup - ](T_TFlex_Model_Data_Filters_TermGroup.md)

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)