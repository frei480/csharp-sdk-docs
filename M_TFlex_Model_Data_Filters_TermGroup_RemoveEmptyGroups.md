

Руководство по T-FLEX CAD Open API

# TermGroupRemoveEmptyGroups - метод  
    
Удаляет из текущей группы элементы, которые являются пустыми группами

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public List<TermGroup> RemoveEmptyGroups(
	bool recursive = true
)
```




#### Параметры

recursive [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean) (Optional)
    Значение true, если требуется удалять элементы в дочерних группах; в противном случае - значение false

#### Возвращаемое значение

[List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[TermGroup](T_TFlex_Model_Data_Filters_TermGroup.md)Список групп условий, удалённых в результате операции

#### Ссылки

[TermGroup - ](T_TFlex_Model_Data_Filters_TermGroup.md)

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)