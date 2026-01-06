

Руководство по T-FLEX CAD Open API

# RowElementGetSourceFragmentIdChain - метод  
    
Список идентификаторов фрагментов, из которых поднят элемент. Если элемент не поднят из фрагмента, то возвращается пустой перечислитель.

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public IEnumerable<ObjectId> GetSourceFragmentIdChain(
	bool fragment3d
)
```




#### Параметры

fragment3d [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Возвращать идентификаторы для 3D фрагментов

#### Возвращаемое значение

[IEnumerable](https://learn.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1)[ObjectId](T_TFlex_Model_ObjectId.md)

#### Ссылки

[RowElement - ](T_TFlex_Model_RowElement.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)