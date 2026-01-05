

Руководство по T-FLEX CAD Open API

# FilterOwnerExtensionsGetSelectionFilterButtonState - метод  
  
---  
  
Получить состояние кнопки селекции

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static bool GetSelectionFilterButtonState(
	this IFilterOwner owner,
	ObjectType objectType,
	ref bool checked,
	ref bool disabled
)
```
```vb
<ExtensionAttribute>
Public Shared Function GetSelectionFilterButtonState ( 
	owner As IFilterOwner,
	objectType As ObjectType,
	ByRef checked As Boolean,
	ByRef disabled As Boolean
) As Boolean
```
```cpp
public:
[ExtensionAttribute]
static bool GetSelectionFilterButtonState(
	IFilterOwner^ owner, 
	ObjectType objectType, 
	bool% checked, 
	bool% disabled
)
```


#### Параметры

owner [IFilterOwner](T_TFlex_Command_IFilterOwner.md)
    
objectType [ObjectType](T_TFlex_Model_ObjectType.md)
    Тип модельного объекта для которого требуется включить селекцию
checked [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Кнопка селектера активирована
disabled [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Кнопка селектора недоступна для изменения

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [IFilterOwner](T_TFlex_Command_IFilterOwner.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[FilterOwnerExtensions - ](T_TFlex_Command_FilterOwnerExtensions.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)