

Руководство по T-FLEX CAD Open API

# ProductStructureGetRowElementGroups(Int32) - метод  
  
---  
  
Получить группы элементов структуры изделия

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ICollection<RowElementGroup> GetRowElementGroups(
	int groupingIndex
)
```
```vb
Public Function GetRowElementGroups ( 
	groupingIndex As Integer
) As ICollection(Of RowElementGroup)
```
```cpp
public:
ICollection<RowElementGroup^>^ GetRowElementGroups(
	int groupingIndex
)
```


#### Параметры

groupingIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс представления, используемого для группировки и объединения элементов

#### Возвращаемое значение

[ICollection](https://learn.microsoft.com/dotnet/api/system.collections.generic.icollection-1)[RowElementGroup](T_TFlex_Model_RowElementGroup.md)

#### Ссылки

[ProductStructure - ](T_TFlex_Model_ProductStructure.md)

[GetRowElementGroups - перегрузка](Overload_TFlex_Model_ProductStructure_GetRowElementGroups.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)