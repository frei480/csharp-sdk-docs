

Руководство по T-FLEX CAD Open API

# FilterOwnerExtensionsShowSelectionFilterButton - метод  
    
Показать кнопку фильтра селекции

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static void ShowSelectionFilterButton(
	this IFilterOwner owner,
	ObjectType objectType,
	bool show
)
```
```vb
<ExtensionAttribute>
Public Shared Sub ShowSelectionFilterButton ( 
	owner As IFilterOwner,
	objectType As ObjectType,
	show As Boolean
)
```
```cpp
public:
[ExtensionAttribute]
static void ShowSelectionFilterButton(
	IFilterOwner^ owner, 
	ObjectType objectType, 
	bool show
)
```


#### Параметры

owner [IFilterOwner](T_TFlex_Command_IFilterOwner.md)
    
objectType [ObjectType](T_TFlex_Model_ObjectType.md)
    Тип модельного объекта для которого требуется включить селекцию
show [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Добавить фильтр

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [IFilterOwner](T_TFlex_Command_IFilterOwner.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[FilterOwnerExtensions - ](T_TFlex_Command_FilterOwnerExtensions.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)