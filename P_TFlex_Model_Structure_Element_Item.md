

Руководство по T-FLEX CAD Open API

# ElementItem(Guid) - свойство  
  
---  
**Пространство имён:** [TFlex.Model.Structure](N_TFlex_Model_Structure.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ElementValue this[
	Guid parameterId
] { get; }
```
```vb
Public ReadOnly Default Property Item ( 
	parameterId As Guid
) As ElementValue
	Get
```
```cpp
public:
property ElementValue^ default[Guid parameterId] {
	ElementValue^ get (Guid parameterId);
}
```


#### Параметры

parameterId [Guid](https://learn.microsoft.com/dotnet/api/system.guid)
    

#### Значение свойства

[ElementValue](T_TFlex_Model_Structure_ElementValue.md)

#### Ссылки

[Element - ](T_TFlex_Model_Structure_Element.md)

[Item - перегрузка](Overload_TFlex_Model_Structure_Element_Item.md)

[TFlex.Model.Structure - пространство имён](N_TFlex_Model_Structure.md)