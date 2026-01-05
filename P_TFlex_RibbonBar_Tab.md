

Руководство по T-FLEX CAD Open API

# RibbonBarTab - свойство  
  
---  
  
i-ая вкладка этой ленты

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public RibbonTab this[
	int i
] {
	[ObsoleteAttribute("This property is obsolete and will be removed. Please use 'GetTab' method.")]
	get;
 }
```
```vb
Public ReadOnly Property Tab ( 
	i As Integer
) As RibbonTab
	<ObsoleteAttribute("This property is obsolete and will be removed. Please use 'GetTab' method.")>
	Get
```
```cpp
public:
property RibbonTab^ Tab[int i] {
	[ObsoleteAttribute(L"This property is obsolete and will be removed. Please use 'GetTab' method.")]
	RibbonTab^ get (int i);
}
```


#### Параметры

i [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    

#### Значение свойства

[RibbonTab](T_TFlex_RibbonTab.md)

#### Ссылки

[RibbonBar - ](T_TFlex_RibbonBar.md)

[TFlex - пространство имён](N_TFlex.md)