

Руководство по T-FLEX CAD Open API

# SelectionContainerExtensionsGetObjectIdChains(SelectionContainer) - метод  
  **Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static IEnumerable<ObjectIdChain> GetObjectIdChains(
	this SelectionContainer A_0
)
```
```vb
<ExtensionAttribute>
Public Shared Function GetObjectIdChains ( 
	A_0 As SelectionContainer
) As IEnumerable(Of ObjectIdChain)
```
```cpp
public:
[ExtensionAttribute]
static IEnumerable<ObjectIdChain^>^ GetObjectIdChains(
	SelectionContainer^ A_0
)
```


#### Параметры

A_0 [SelectionContainer](T_TFlex_Model_SelectionContainer.md)
    

#### Возвращаемое значение

[IEnumerable](https://learn.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1)[ObjectIdChain](T_TFlex_Model_ObjectIdChain.md)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [SelectionContainer](T_TFlex_Model_SelectionContainer.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[SelectionContainerExtensions - ](T_TFlex_Model_SelectionContainerExtensions.md)

[GetObjectIdChains - перегрузка](Overload_TFlex_Model_SelectionContainerExtensions_GetObjectIdChains.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)