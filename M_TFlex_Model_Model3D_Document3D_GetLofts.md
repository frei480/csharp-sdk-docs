

Руководство по T-FLEX CAD Open API

# Document3DGetLofts - метод  
  
---  
  
**Примечание: Данный API устарел.**

Контейнер операций "По сечениям"

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This property is obsolete and will be removed. Please use 'GetLoftOperations' method.", 
	true)]
public static ICollection<Loft> GetLofts(
	this Document document
)
```
```vb
<ExtensionAttribute>
<ObsoleteAttribute("This property is obsolete and will be removed. Please use 'GetLoftOperations' method.", 
	true)>
Public Shared Function GetLofts ( 
	document As Document
) As ICollection(Of Loft)
```
```cpp
public:
[ExtensionAttribute]
[ObsoleteAttribute(L"This property is obsolete and will be removed. Please use 'GetLoftOperations' method.", 
	true)]
static ICollection<Loft^>^ GetLofts(
	Document^ document
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    

#### Возвращаемое значение

[ICollection](https://learn.microsoft.com/dotnet/api/system.collections.generic.icollection-1)[Loft](T_TFlex_Model_Model3D_Loft.md)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [Document](T_TFlex_Model_Document.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[Document3D - ](T_TFlex_Model_Model3D_Document3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)