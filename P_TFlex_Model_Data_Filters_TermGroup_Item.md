

Руководство по T-FLEX CAD Open API

# TermGroupItem - свойство  
    
Возвращает элемент, находящийся в группе условий по указанному индексу

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public TermGroupItem this[
	int index
] { get; set; }
```
```vb
Public Default Property Item ( 
	index As Integer
) As TermGroupItem
	Get
	Set
```
```cpp
public:
virtual property TermGroupItem^ default[int index] {
	TermGroupItem^ get (int index) sealed;
	void set (int index, TermGroupItem^ value) sealed;
}
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс элемента в группе

#### Возвращаемое значение

[TermGroupItem](T_TFlex_Model_Data_Filters_TermGroupItem.md)Элемент, находящийся в группе условий по указанному индексу

#### Реализации

[IListTItemInt32](https://learn.microsoft.com/dotnet/api/system.collections.generic.ilist-1.item)

#### Ссылки

[TermGroup - ](T_TFlex_Model_Data_Filters_TermGroup.md)

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)