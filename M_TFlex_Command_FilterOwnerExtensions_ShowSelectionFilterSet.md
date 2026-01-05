

Руководство по T-FLEX CAD Open API

# FilterOwnerExtensionsShowSelectionFilterSet - метод  
  
---  
  
Показать конфигурацию селектора

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static void ShowSelectionFilterSet(
	this IFilterOwner owner,
	SelectorSetType setType
)
```
```vb
<ExtensionAttribute>
Public Shared Sub ShowSelectionFilterSet ( 
	owner As IFilterOwner,
	setType As SelectorSetType
)
```
```cpp
public:
[ExtensionAttribute]
static void ShowSelectionFilterSet(
	IFilterOwner^ owner, 
	SelectorSetType setType
)
```


#### Параметры

owner [IFilterOwner](T_TFlex_Command_IFilterOwner.md)
    
setType [SelectorSetType](T_TFlex_Command_SelectorSetType.md)
    Набор для селекции

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [IFilterOwner](T_TFlex_Command_IFilterOwner.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[FilterOwnerExtensions - ](T_TFlex_Command_FilterOwnerExtensions.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)