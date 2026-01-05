

Руководство по T-FLEX CAD Open API

# TFXmlHelperWriteBoolAttribute - метод  
  
---  
**Пространство имён:** [TFlex.Model.Data](N_TFlex_Model_Data.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public static void WriteBoolAttribute(
	this XmlWriter writer,
	string attrName,
	bool bVal
)
```
```vb
<ExtensionAttribute>
Public Shared Sub WriteBoolAttribute ( 
	writer As XmlWriter,
	attrName As String,
	bVal As Boolean
)
```
```cpp
public:
[ExtensionAttribute]
static void WriteBoolAttribute(
	XmlWriter^ writer, 
	String^ attrName, 
	bool bVal
)
```


#### Параметры

writer [XmlWriter](https://learn.microsoft.com/dotnet/api/system.xml.xmlwriter)
    
attrName [String](https://learn.microsoft.com/dotnet/api/system.string)
    
bVal [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [XmlWriter](https://learn.microsoft.com/dotnet/api/system.xml.xmlwriter). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[TFXmlHelper - ](T_TFlex_Model_Data_TFXmlHelper.md)

[TFlex.Model.Data - пространство имён](N_TFlex_Model_Data.md)