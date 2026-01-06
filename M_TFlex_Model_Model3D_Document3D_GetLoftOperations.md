

Руководство по T-FLEX CAD Open API

# Document3DGetLoftOperations - метод  
    
Контейнер операций "По сечениям"

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static ICollection<LoftOperation> GetLoftOperations(
	this Document document
)
```
```vb
<ExtensionAttribute>
Public Shared Function GetLoftOperations ( 
	document As Document
) As ICollection(Of LoftOperation)
```
```cpp
public:
[ExtensionAttribute]
static ICollection<LoftOperation^>^ GetLoftOperations(
	Document^ document
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    

#### Возвращаемое значение

[ICollection](https://learn.microsoft.com/dotnet/api/system.collections.generic.icollection-1)[LoftOperation](T_TFlex_Model_Model3D_LoftOperation.md)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [Document](T_TFlex_Model_Document.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[Document3D - ](T_TFlex_Model_Model3D_Document3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)