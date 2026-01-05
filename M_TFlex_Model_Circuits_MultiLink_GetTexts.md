

Руководство по T-FLEX CAD Open API

# MultiLinkGetTexts(Boolean, DesignationType) - метод  
  
---  
**Пространство имён:** [TFlex.Model.Circuits](N_TFlex_Model_Circuits.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public override IEnumerable<Tuple<MultilineText, string>> GetTexts(
	bool edit,
	DesignationType type
)
```
```vb
Public Overrides Function GetTexts ( 
	edit As Boolean,
	type As DesignationType
) As IEnumerable(Of Tuple(Of MultilineText, String))
```
```cpp
public:
virtual IEnumerable<Tuple<MultilineText^, String^>^>^ GetTexts(
	bool edit, 
	DesignationType type
) override
```


#### Параметры

edit [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
type [DesignationType](T_TFlex_Model_Circuits_DesignationType.md)
    

#### Возвращаемое значение

[IEnumerable](https://learn.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1)[Tuple](https://learn.microsoft.com/dotnet/api/system.tuple-2)[MultilineText](T_TFlex_Model_Model2D_MultilineText.md), [String](https://learn.microsoft.com/dotnet/api/system.string)

#### Ссылки

[MultiLink - ](T_TFlex_Model_Circuits_MultiLink.md)

[GetTexts - перегрузка](Overload_TFlex_Model_Circuits_MultiLink_GetTexts.md)

[TFlex.Model.Circuits - пространство имён](N_TFlex_Model_Circuits.md)