

Руководство по T-FLEX CAD Open API

# Document3DGetCountTopologyReferences - метод  
  
---  
  
**Примечание: Данный API устарел.**

Количество топологических ссылок

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This property is obsolete. Please use 'GetTopologyReferenceCount' method.")]
public static ulong GetCountTopologyReferences(
	this Document document
)
```
```vb
<ExtensionAttribute>
<ObsoleteAttribute("This property is obsolete. Please use 'GetTopologyReferenceCount' method.")>
Public Shared Function GetCountTopologyReferences ( 
	document As Document
) As ULong
```
```cpp
public:
[ExtensionAttribute]
[ObsoleteAttribute(L"This property is obsolete. Please use 'GetTopologyReferenceCount' method.")]
static unsigned long long GetCountTopologyReferences(
	Document^ document
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    

#### Возвращаемое значение

[UInt64](https://learn.microsoft.com/dotnet/api/system.uint64)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [Document](T_TFlex_Model_Document.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[Document3D - ](T_TFlex_Model_Model3D_Document3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)