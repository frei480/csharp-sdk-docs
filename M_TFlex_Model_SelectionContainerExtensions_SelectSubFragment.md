

Руководство по T-FLEX CAD Open API

# SelectionContainerExtensionsSelectSubFragment(SelectionContainer, Fragment3D, IEnumerableObjectId) - метод  
  **Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static void SelectSubFragment(
	this SelectionContainer selCont,
	Fragment3D fragment,
	IEnumerable<ObjectId> fragmentIdChain
)
```
```vb
<ExtensionAttribute>
Public Shared Sub SelectSubFragment ( 
	selCont As SelectionContainer,
	fragment As Fragment3D,
	fragmentIdChain As IEnumerable(Of ObjectId)
)
```
```cpp
public:
[ExtensionAttribute]
static void SelectSubFragment(
	SelectionContainer^ selCont, 
	Fragment3D^ fragment, 
	IEnumerable<ObjectId^>^ fragmentIdChain
)
```


#### Параметры

selCont [SelectionContainer](T_TFlex_Model_SelectionContainer.md)
    
fragment [Fragment3D](T_TFlex_Model_Model3D_Fragment3D.md)
    
fragmentIdChain [IEnumerable](https://learn.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1)[ObjectId](T_TFlex_Model_ObjectId.md)
    

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [SelectionContainer](T_TFlex_Model_SelectionContainer.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[SelectionContainerExtensions - ](T_TFlex_Model_SelectionContainerExtensions.md)

[SelectSubFragment - перегрузка](Overload_TFlex_Model_SelectionContainerExtensions_SelectSubFragment.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)